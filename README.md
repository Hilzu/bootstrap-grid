# bootstrap-grid
Standalone version of Bootstrap 3 grid system.

## Why?

Bootstrap 3 contains a best of breed responsive grid system that is useful without the rest of bootstrap. This project
builds a standalone version of it with just the container, row and columns classes.

## How to use the grid?

See the [grid system documentation][grid] in Bootstrap's own documentation page.

## How do I use this project?

* Download the `grid.css` file and include it in your project.
* Install this package with npm and
  * include `index.less` in your less build
  * include/require `grid.css` in your stylesheets
* Any way you can think of really.

## What's included?

The following classes are included in this project:

* clearfix
* container
* container-fluid
* row
* All the col classes: col-(xs|sm|md|lg)-\[(push|pull|offset)-](1-12)

## How do I build this?

Install dependencies

    $ npm install

Run build

    $ npm run build

The file `grid.css` is generated that contains the whole grid system.

[grid]: http://getbootstrap.com/css/#grid
