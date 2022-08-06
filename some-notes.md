---
layout: main
---

# SIDE NOTES FOR MYSELF.

Whenever i will see my own written file, i am gonna know all about this project
or jekyll build in future.

_NOTE: Read this file, but don't rely on this. This is my guide_

## \_ this thing:

Its called underscore, all the file, folders that starts with _ aren't gonna render. These are now "Bundle Files".
Note that, i made a new file called "\_side-notes.md", it starts with underscore. Try it, remove _ from the start, you will see what i was talking about.
If you remove underscore, it gonna render on this address: http://127.0.0.1:4000/side-notes.md.

Also, you can see its file in the *\_post* folder. If you rename it again, and add \_ its gonna remove from the \_post folder. You cant access this file now by http://127.0.0.1:4000/side-notes.md.

## Gemfile:

So as you know(I suppose), jekyll is a ruby gem. In order to make a jekyll project we have to make a Gemfile.
This file is _THE HEART_ of jekyll project. It includes:

- Project Dependencies.
- Gems we gonna use
- Needed gems for the project.

Now here comes a question, How we can fetch these gems?
The answer is simple, we have give a source, gem name and its version(If you need specific version).

_NOTE: As my mentor said, i am gonna use following Gems in all projects, until i need some other functionality in my project_.

    source "https://rubygems.org"

    gem 'jekyll', '~> 4.2'
    gem 'webrick'
    gem 'wdm', '>= 0.1.0' if Gem.win_platform?
    gem 'eventmachine', '~> 1.2.7'

## Gemfile.lock:

This file came when we run serve command. Its make the gems useable for the project. It compile the gems and directly linked it with the project.

We can see all the gems and there dependencies including there versions in this file.

_NOTE: DON"T CHANGE ANYTHING IN THOSE FILES, WHOSE NAME STARTS FROM UNDERSCORE( \_ ) UNLESS YOU KNOW WHAT YOU ARE DOING_

## Pages:

All the .html files that are present in our _ROOT DIR_ are called pages. These are the files that gonna render in the end. User can only see these files on their browser.
You can make as many pages as you want.
Like:

- about.html
- contact.html
- services.html
- team.html
- and many more...

_NOTE: Now we have discussed all the ROOT FILES, lets move to ROOT FOLDERS_

## ROOT FOLDERS:

All the folders that are starting with underscore are the main jekyll project folders.

_NOTE: I am going to define these by a sequence, this is the way we start our project, after including all gems and there dependencies_

1. \_layouts:

   Layouts folder is the "THEME" of a webpage. In simple word what we actually want a page look like decide in layouts.
   I am going to make a layout called "main" layout.
   We will make it with extension name "main.html". Because its a HTML page and browser only understand html doctype.

- So i made a layout, made it just like simple html sheet.
- In title, i used this "{{ page.title }}".
- So the it is fetching the title from page.
- It means, it doest matter how many page you have.
- Every new page has its own title. If we dont use this, we have to make new layout for every page. If we are gonna do that, than why using jekyll?.

         From Where it gonna take title?
         So, we have to give each page a title in the start. Its really easy, instead of writing whole HTML meta data, just use simple two line code.

2. _include folder:
    In this folder we add all the things we are gonna use in the pages. We just have to write only first time then we can use this in any page. like what we can add in include folder?
    Here is a list:
- Header
- Heros
- Cover
- Nav bars
- Footer
- Things like that

So all the things that we are gonna use in all pages, we can make a include partial of it and just use it instead of writing the whole HTML content. Copy paste it again and again. 


