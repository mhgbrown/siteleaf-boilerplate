# Siteleaf Boilerplate

This is Ruby-based starter project for sites backed by [Siteleaf **v1**](http://www.siteleaf.com/).

## Features

* [Sass](https://www.ruby-lang.org/en/downloads/) + [Compass](http://compass-style.org/)
* [Jammit](http://documentcloud.github.io/jammit/) + [Uglify](https://github.com/mishoo/UglifyJS)
* [Normalize.css](https://necolas.github.io/normalize.css/)
* [jQuery](https://jquery.com/)
* [HTML5 Shiv](https://github.com/aFarkas/html5shiv)
* [humans.txt](http://humanstxt.org/)
* Facebook and Twitter meta tags
* 404 page that redirects home

## Getting Started

Make sure you have [Ruby 2.2.4](https://www.ruby-lang.org/en/downloads/) installed or take a look at the Gemfile to change the version to your taste.

* Add your ```:site_id``` to ```config.ru```. You can find it in part of the management interface URL: manage.siteleaf.com/sites/**:site_id**/pages
* ```bundle install```
* ```siteleaf auth```
* ```guard```
* ```siteleaf server```
* Develop!

And don't forget to push your theme changes to Siteleaf!
* ```siteleaf push theme```
