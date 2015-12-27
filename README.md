# One-stop Ruby on Rails: Build Web Applications from Scratch

App Demo:  
http://yelpdemo.herokuapp.com/

Video Course link:  
https://www.udemy.com/build-etsy-yelp-craigslist-and-a-web-scraper-from-scratch/

If you will register on udemy.com and click on "Start Free Preview", аfter some period you can receive (by email) big discount on this course.

____


<br/>

### Prepare Linux Environment for Development

    # yum install -y \
    which \
    tar \
    curl \
    openssl-devel \
    git \
    gcc


    # useradd \
    -d /home/developer \
    -m developer

    # passwd developer


    # mkdir /rails_projects
    # chown -R developer /rails_projects/


    # su - developer

    $ cd ~/
    $ git clone git://github.com/sstephenson/rbenv.git .rbenv
    $ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bashrc
    $ echo 'eval "$(rbenv init -)"' >> ~/.bashrc
    $ exec $SHELL


    $ git clone git://github.com/sstephenson/ruby-build.git ~/.rbenv/plugins/ruby-build
    $ echo 'export PATH="$HOME/.rbenv/plugins/ruby-build/bin:$PATH"' >> ~/.bashrc
    $ exec $SHELL

    $ rbenv install --list

    $ rbenv install 2.2.3
    $ rbenv global 2.2.3
    $ ruby -v
    ruby 2.2.3p173 (2015-08-18 revision 51636) [x86_64-linux]

    $ gem install bundler
    $ rbenv rehash
    $ bundle -v
    Bundler version 1.11.2

    $ gem install rails --no-ri --no-rdoc
    $ rbenv rehash
    $ rails -v
    Rails 4.2.5

    $ rails new .
    $ rails server -b 0.0.0.0 -p 3000

    http://localhost:3000/

<br/>

### 02 Create our Website

005 Add Our First Pages

    $ rails generate controller Pages about contact

 http://localhost:3000/pages/about
 http://localhost:3000/pages/contact
