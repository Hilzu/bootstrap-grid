# bootstrap-grid

Standalone version of Bootstrap 3 grid system. See the [test][test.html] file for a demo.

## Why?

Bootstrap 3 contains a best of breed responsive grid system. It's useful without all the rest of Bootstrap. This project
contains a standalone version of it with related utility classes.

## How to use the grid system?

See Bootstrap's [grid system][grid] and [responsive utilities][responsive] documentation.

## How do I use this project?

You have several choices:

1. Download the `grid.css` or `grid.min.css` file from the `dist` folder and include it in your project.
2. Install this package with npm and include/require `grid.css` or `grid.min.css` directly from
`node_modules`.
3. If you are using webpack with `css-loader` you can just `require("bootstrap-grid")`.
4. Any other way you can think of really.

The Bootstrap grid system expects the columns and containers to have `box-sizing: border-box` set.
The `grid.css` file doesn't have that rule because it's set in Bootstrap's `scaffolding.less` file that
also includes lot's of other modifications to global element styles.
We could set the rule for you globally but a small library like this shouldn't include such things.

Because of this you must set it yourself using `* { box-sizing: border-box; }`.
You can also set it separately for every Bootstrap class but that's not really fun...

You can check the [test][test.html] file for an example how to use and setup the grid.

## What's included?

The following classes are included:

* clearfix
* container
* container-fluid
* row
* All the col classes from col-xs-1 to col-lg-12 including push, pull and offset versions: `col-(xs-lg)-[(push|pull|offset)-](1-12)`
* hidden classes for all breakpoints: `hidden-(xs-lg|print)`
* visible classes for all breakpoints and display values: `visible-(xs-lg|print)-(block|inline|inline-block)`.
* `visible-(xs-lg|print)` are also included but they are deprecated as of Bootstrap v3.2.0 and should not be used.

## How do I build this?

Install dependencies

    $ npm install

Run build

    $ npm run build

`grid.css` and the minified `grid.min.css` are generated.

[grid]: http://getbootstrap.com/css/#grid
[responsive]: http://getbootstrap.com/css/#responsive-utilities
[test.html]: https://rawgit.com/Hilzu/bootstrap-grid/master/test.html
