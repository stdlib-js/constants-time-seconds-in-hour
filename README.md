<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# Seconds in an Hour

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Number of seconds in an hour.

<section class="installation">

## Installation

```bash
npm install @stdlib/constants-time-seconds-in-hour
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm` branch][esm-url].
-   If you are using Deno, visit the [`deno` branch][deno-url].
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd` branch][umd-url].

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

</section>

<section class="usage">

## Usage

```javascript
var SECONDS_IN_HOUR = require( '@stdlib/constants-time-seconds-in-hour' );
```

#### SECONDS_IN_HOUR

Number of seconds in an hour.

```javascript
var bool = ( SECONDS_IN_HOUR === 3600 );
// returns true
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   The value is a generalization and does **not** take into account inaccuracies due to daylight savings conventions, crossing timezones, or other complications with time and dates. 

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var randu = require( '@stdlib/random-base-randu' );
var roundn = require( '@stdlib/math-base-special-roundn' );
var SECONDS_IN_HOUR = require( '@stdlib/constants-time-seconds-in-hour' );

var secs;
var hrs;
var i;

function hrs2secs( hrs ) {
    return hrs * SECONDS_IN_HOUR;
}

for ( i = 0; i < 10; i++ ) {
    hrs = roundn( randu()*20.0, -2 );
    secs = hrs2secs( hrs );
    console.log( '%d hours => %d seconds', hrs, secs );
}
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/constants-time-seconds-in-hour.svg
[npm-url]: https://npmjs.org/package/@stdlib/constants-time-seconds-in-hour

[test-image]: https://github.com/stdlib-js/constants-time-seconds-in-hour/actions/workflows/test.yml/badge.svg?branch=v0.0.8
[test-url]: https://github.com/stdlib-js/constants-time-seconds-in-hour/actions/workflows/test.yml?query=branch:v0.0.8

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/constants-time-seconds-in-hour/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/constants-time-seconds-in-hour?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/constants-time-seconds-in-hour.svg
[dependencies-url]: https://david-dm.org/stdlib-js/constants-time-seconds-in-hour/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/constants-time-seconds-in-hour/tree/deno
[umd-url]: https://github.com/stdlib-js/constants-time-seconds-in-hour/tree/umd
[esm-url]: https://github.com/stdlib-js/constants-time-seconds-in-hour/tree/esm
[branches-url]: https://github.com/stdlib-js/constants-time-seconds-in-hour/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/constants-time-seconds-in-hour/main/LICENSE

</section>

<!-- /.links -->
