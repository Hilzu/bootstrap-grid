# bootstrap-grid
Standalone version of Bootstrap 3 grid system.

## Why?

Bootstrap 3 contains a best of breed responsive grid system. It's useful without all the rest of Bootstrap. This project
contains a standalone version of it with just the grid and related utility classes.

## How to use the grid?

See Bootstrap's [grid system][grid] and [responsive utilities][responsive] documentation.

## How do I use this project?

* Download the `grid.css` or `grid.min.css` file and include it in your project.
* Install this package with npm and
  * include/require `grid.css` or `grid.min.css` in your stylesheets.
  * include `index.less` in your less build. Note that this makes all the variables and mixins from Bootstrap available to your less files. You must build the `index.less` separately if you don't want that.
* Any other way you can think of really.

## What's included?

The following classes are included:

* clearfix
* container
* container-fluid
* row
* All the col classes from col-xs-1 to col-lg-12 including push, pull and offset versions: `col-(xs-lg)-[(push|pull|offset)-](1-12)`
* hidden classes for all breakpoints: `hidden-(xs-lg|print)`
* visible classes for all breakpoints and columns: `visible-(xs-lg|print)-(block|inline|inline-block)`.
* `visible-(xs-lg|print)` are also included but they are deprecated as of bootstrap v3.2.0 and should not be used.

## How do I build this?

Install dependencies

    $ npm install

Run build

    $ npm run build

`grid.css` and a minified `grid.min.css` are generated.

[grid]: http://getbootstrap.com/css/#grid
[responsive]: http://getbootstrap.com/css/#responsive-utilities
