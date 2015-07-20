# bootstrap-grid
Standalone version of Bootstrap 3 grid system.

## Why?

Bootstrap 3 contains a best of breed responsive grid system. It's useful without all the rest of Bootstrap. This project
builds a standalone version of it with just the container, row and columns classes.

## How to use the grid?

See [Bootstrap grid system documentation][grid].

## How do I use this project?

* Download the `grid.css` file and include it in your project.
* Install this package with npm and
  * include/require `grid.css` in your stylesheets.
  * include `index.less` in your less build. Note that this makes all the variables and mixins from Bootstrap available to your less files. You must build the `index.less` separately if you don't want that.
* Any other way you can think of really.

## What's included?

The following classes are included:

* clearfix
* container
* container-fluid
* row
* All the col classes from col-xs-1 to col-lg-12 including push, pull and offset versions: col-(xs|sm|md|lg)-\[(push|pull|offset)-](1-12)

## How do I build this?

Install dependencies

    $ npm install

Run build

    $ npm run build

The file `grid.css` is generated containing the grid system.

[grid]: http://getbootstrap.com/css/#grid
