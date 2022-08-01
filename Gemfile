source "https://rubygems.org"

gem 'jekyll', '~> 4.2'
# Jekyll's core source
gem 'webrick'
# Webrick is what runs the server to host our project while development
gem 'wdm', '>= 0.1.0' if Gem.win_platform?
# WDM is what controls the livereload and project publishing logic
platforms :mingw, :x64_mingw, :mswin, :jruby do
    gem "tzinfo", ">= 1", "< 3"
    gem "tzinfo-data"
  end
# This is just for windows OS timezone issue fix. If you don't have it, when developing in windows, your posts time will be conflicted
gem 'eventmachine', '~> 1.2.7'
# Something specific to ruby for jekyll's core functionality hooks