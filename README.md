#concrete

[![Bower version][bower-img]][bower-url]
[![Build][travis-img]][travis-url]
[![Dependency Status][david-img]][david-url]

  [bower-img]: https://img.shields.io/bower/v/concrete.svg
  [bower-url]: https://github.com/roeldev/concrete
  [travis-img]: https://img.shields.io/travis/roeldev/concrete/master.svg
  [travis-url]: https://travis-ci.org/roeldev/concrete
  [david-img]: https://david-dm.org/roeldev/concrete/dev-status.svg
  [david-url]: https://david-dm.org/roeldev/concrete#info=devDependencies

**Sassy CSS framework**

Includes functions/mixins for media queries/breakpoints, flexible responsive grids, effects and shapes. Also included are some functions/mixins to more easily debug your own custom Sass :)


## Main features
- Easy configuration of media queries and breakpoints. Set them the way you want or need them.
- 10, 11 or 12 columns? It doesn't matter, you define the widths and how each column reacts to different breakpoints.
- Cool transition mixin! Just define the easing, time and delay properties in the `_transitions.scss` settings file and you're ready to go. Now all your transitions automatically have the same default properties. You can even create multiple groups for different transitions if you need them.
- Lots of type check functions, sort functions, and more list/map related functions!
- Includes [normalize.css v3.0.3][url-normalize] and more useful style classes.
- Some basic shapes and effects, such as hexagons, triangles, gradients and fancy text shadows.
- Extended debug functions and mixins. Output variables in the console or the compiled CSS to see what their actual values are. This makes developing your own stuff even easier :)

## Installation
Either [download the latest release][url-project-releases] or [install with Bower][url-bower-install]:
```sh
bower install --save concrete
```

## How to get started
1. Copy the `starter` folder to your project.
2. Update the `@import` rules in `_concrete.scss` that start with `../src/`. Point them to the right file(s) in the `src/` folder of this package, relative to your project's folder. Example: `../bower_components/concrete/src/`.
3. Change the default values and/or settings variables in the files in the `concrete` folder so it suits your project.
4. You can rename `main.scss` to whatever you want and place your own `@import` rules or custom CSS/SCSS in this file.

> Check the SassDoc documentation in the `sassdoc/` folder for all available functions.
> You can rename `main.scss` to whatever you want. This file is only used as a small starter for your project.
> Please note that removing any of the `$concrete-` prefixed variables will break the framework.

In `_basics.scss` you can remove (by adding comments) any predefined style classes wich you don't plan to use. This will keep the compiled CSS file cleaner and smaller.


## What's included
Within the package you'll find the following folder structure:
```
concrete/
├── docs/
│   ├── ...
│   └── index.html
├── examples/
│   └── ...
├── src/
│   └── ...
├── starter/
│   ├── concrete/
│   │   └── ...
│   ├── _concrete.scss
│   └── main.scss
└── test/
    └── ...
```
All framework related sources files are located in the `src/` folder. It is recommended to check the source to see how the framework works from the inside.

In `examples/` and `examples/scss/` you'll find some basic usage examples. The folder `examples/css/` contains the CSS files wich are compiled from the SCSS files in the `examples/scss/` folder.

The documentation is generated with [SassDoc][url-sassdoc]. Just open the `docs/index.html` file the see a description and wich arguments are expected per function.

Pretty much all functions and mixins have tests in the `test/` dir. Tests are performed with [True][url-true] and [Mocha][url-mocha].


## License
[GPL-2.0+](LICENSE) © 2014-2016 [Roel Schut](http://roelschut.nl)


[url-project-main]: https://github.com/roeldev/concrete
[url-project-releases]: https://github.com/roeldev/concrete/releases
[url-normalize]: https://github.com/necolas/normalize.css/
[url-bower-install]: http://bower.io/
[url-sassdoc]: http://sassdoc.com/
[url-true]: https://github.com/ericam/true
[url-mocha]: http://mochajs.org/
