# APPUiO Website

Uses middleman to generate static HTML

* Documentation: https://middlemanapp.com/

* Index is here: /localizable/index.html.erb

Optimize images before build:

    image_optim source/images/*.{jpg,png,gif,svg}

## Prerequisites

* Ruby v2.2.2
* Middleman

Once you have Ruby and RubyGems up and running, execute the following from the command line:

    $ gem install middleman
    $ gem install bundle

This will install Middleman, its dependencies and the command-line tools for using Middleman.

First of all, be sure to run under ```Ruby v2.2.2``` at least, then:

    $ bundle install

## Setup Development environment:
    
    $ middleman

## Build the static pages:

    $ bundle exec middleman build
    
    
## Deploy the Website with rsync

    $ rsync -a ./build/ user@example.com:~/path
