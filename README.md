# bootstrap-grid
Standalone version of Bootstrap 3 grid system. See the [test][test.html] file for a demo.

## Why?

Bootstrap 3 contains a best of breed responsive grid system. It's useful without all the rest of Bootstrap. This project
contains a standalone version of it with just the grid and related utility classes.

## How to use the grid system?

See Bootstrap's [grid system][grid] and [responsive utilities][responsive] documentation.

## How do I use this project?

You have several choices:

1. (Recommended) Download the `grid.css` or `grid.min.css` file and include it in your project.
2. Install this package with npm and
  * (Recommended) Include/require `grid.css` or `grid.min.css` to your project.
  * Include `index.less` in your less build. Note that this makes all the variables and mixins from Bootstrap available to your less files. You must build the `index.less` separately if you don't want that.
3. Any other way you can think of really.

The bootstrap grid system expects the columns and containers to have `box-sizing: border-box` set.
The `grid.css` file doesn't have that rule because it's set in bootstrats scaffolding.less file that also includes lot's of other modifications to global element styles.
A small library like this shouldn't include such things.

Because of this you must set it yourself using `* { box-sizing: border-box; }`.
You can also set it separately for every bootstrap class but that's not really fun...

You can check the [example][test.html] file for an example how to use and setup the grid.

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
[test.html]: https://rawgit.com/Hilzu/bootstrap-grid/master/test.html
