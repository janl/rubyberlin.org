
Ruby Berlin e.V. Website README
=======================

In this repository you'll find the website for Ruby Berlin e.V..

Install
-------

Provided you have RVM installed, installation should require **4 Steps**:

    rvm 1.9.3
    rvm gemset create middleman
    gem install bundler
    bundle install

Running
-------

### Building static pages

You can build the site into a `build`-directory:

    bundle exec middleman build

The `build` directory will contain the generated HTML, CSS and JavaScript and
the contents can be uploaded to any standard web server.

### With Pow

Download and install [POW](http://pow.cx/):

    curl get.pow.cx | sh

Then:

    cd ~/.pow
    ln -s /path/to/rubyberlin_website rubyberlin

You will see the generated HTML & CSS by navigating to <http://rubyberlin.dev/>.

### With the built-in server

To run:

    bundle exec middleman server

You will see the generated HTML & CSS by navigating to <http://localhost:4567/>.

Deployment
----------

### Staging

* <http://dev.rubyberlin.org/>
* `bundle exec rake staging deploy`

### Production

* <http://rubyberlin.org/>
* `bundle exec rake production deploy`
