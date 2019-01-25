# gulp-pixrem2 [![NPM version](https://badge.fury.io/js/gulp-pixrem2.png)](http://badge.fury.io/js/gulp-pixrem2) [![Build Status](https://travis-ci.org/nitishd/gulp-pixrem2.png?branch=master)](https://travis-ci.org/nitishd/gulp-pixrem2) [![Coverage Status](https://coveralls.io/repos/github/nitishd/gulp-pixrem2/badge.svg)](https://coveralls.io/github/nitishd/gulp-pixrem2)

> [Pixrem](https://github.com/robwierzbowski/node-pixrem) – A CSS post-processor that generates pixel fallbacks for rem units.

This is an updated version of [gulp-pixrem](https://www.npmjs.com/package/gulp-pixrem) with deprecated code removed .

Issues with the output should be reported on the [Pixrem](https://github.com/robwierzbowski/node-pixrem) issue tracker.

## Installation

~~~ shell
npm install gulp-pixrem2 --save-dev
~~~

## Usage

For usage and options, refer to the official [Pixrem](https://github.com/robwierzbowski/node-pixrem#usage) repository.

## Examples

~~~ javascript
var gulp = require('gulp');
var pixrem = require('gulp-pixrem2');

gulp.task('css', function() {
  gulp.src('css/style.css')
    .pipe(pixrem())
    .pipe(gulp.dest('public/css/'));
});

gulp.task('css', function() {
  gulp.src('css/style.css')
    .pipe(pixrem({ rootValue: '10px' }))
    .pipe(gulp.dest('public/css/'));
});

gulp.task('css', function() {
  gulp.src('css/style.css')
    .pipe(pixrem({
      rootValue: '100%',
      replace: true
    }))
    .pipe(gulp.dest('public/css/'));
});
~~~

## License

The MIT License (MIT)

Copyright (c) 2014 Ellen Gummesson
Copyright (c) 2019 Nitish Kumar

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
