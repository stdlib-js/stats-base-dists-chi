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

# Chi

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Chi distribution.

<section class="installation">

## Installation

```bash
npm install @stdlib/stats-base-dists-chi
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
var chi = require( '@stdlib/stats-base-dists-chi' );
```

#### chi

Chi distribution.

```javascript
var dist = chi;
// returns {...}
```

The namespace contains the following distribution functions:

<!-- <toc pattern="*+(cdf|pdf|mgf|quantile)*"> -->

<div class="namespace-toc">

-   <span class="signature">[`cdf( x, k )`][@stdlib/stats/base/dists/chi/cdf]</span><span class="delimiter">: </span><span class="description">Chi distribution cumulative distribution function.</span>
-   <span class="signature">[`logpdf( x, k )`][@stdlib/stats/base/dists/chi/logpdf]</span><span class="delimiter">: </span><span class="description">evaluate the natural logarithm of the probability density function (PDF) for a chi distribution .</span>
-   <span class="signature">[`pdf( x, k )`][@stdlib/stats/base/dists/chi/pdf]</span><span class="delimiter">: </span><span class="description">Chi distribution probability density function (PDF).</span>
-   <span class="signature">[`quantile( p, k )`][@stdlib/stats/base/dists/chi/quantile]</span><span class="delimiter">: </span><span class="description">Chi distribution quantile function.</span>

</div>

<!-- </toc> -->

The namespace contains the following functions for calculating distribution properties:

<!-- <toc pattern="*+(entropy|kurtosis|mean|median|mode|skewness|stdev|variance)*"> -->

<div class="namespace-toc">

-   <span class="signature">[`entropy( k )`][@stdlib/stats/base/dists/chi/entropy]</span><span class="delimiter">: </span><span class="description">Chi distribution differential entropy.</span>
-   <span class="signature">[`kurtosis( k )`][@stdlib/stats/base/dists/chi/kurtosis]</span><span class="delimiter">: </span><span class="description">Chi distribution excess kurtosis.</span>
-   <span class="signature">[`mean( k )`][@stdlib/stats/base/dists/chi/mean]</span><span class="delimiter">: </span><span class="description">Chi distribution expected value.</span>
-   <span class="signature">[`mode( k )`][@stdlib/stats/base/dists/chi/mode]</span><span class="delimiter">: </span><span class="description">Chi distribution mode.</span>
-   <span class="signature">[`skewness( k )`][@stdlib/stats/base/dists/chi/skewness]</span><span class="delimiter">: </span><span class="description">Chi distribution skewness.</span>
-   <span class="signature">[`stdev( k )`][@stdlib/stats/base/dists/chi/stdev]</span><span class="delimiter">: </span><span class="description">Chi distribution standard deviation.</span>
-   <span class="signature">[`variance( k )`][@stdlib/stats/base/dists/chi/variance]</span><span class="delimiter">: </span><span class="description">Chi distribution variance.</span>

</div>

<!-- </toc> -->

The namespace contains a constructor function for creating a [Chi][chi-distribution] distribution object.

<!-- <toc pattern="*ctor*"> -->

<div class="namespace-toc">

-   <span class="signature">[`Chi( [k] )`][@stdlib/stats/base/dists/chi/ctor]</span><span class="delimiter">: </span><span class="description">Chi distribution constructor.</span>

</div>

<!-- </toc> -->

```javascript
var Chi = require( '@stdlib/stats-base-dists-chi' ).Chi;

var dist = new Chi( 4.0 );

var mu = dist.mean;
// returns ~1.88
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- TODO: better examples -->

<!-- eslint no-undef: "error" -->

```javascript
var objectKeys = require( '@stdlib/utils-keys' );
var chi = require( '@stdlib/stats-base-dists-chi' );

console.log( objectKeys( chi ) );
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

[npm-image]: http://img.shields.io/npm/v/@stdlib/stats-base-dists-chi.svg
[npm-url]: https://npmjs.org/package/@stdlib/stats-base-dists-chi

[test-image]: https://github.com/stdlib-js/stats-base-dists-chi/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/stats-base-dists-chi/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/stats-base-dists-chi/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/stats-base-dists-chi?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/stats-base-dists-chi.svg
[dependencies-url]: https://david-dm.org/stdlib-js/stats-base-dists-chi/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/stats-base-dists-chi/tree/deno
[umd-url]: https://github.com/stdlib-js/stats-base-dists-chi/tree/umd
[esm-url]: https://github.com/stdlib-js/stats-base-dists-chi/tree/esm
[branches-url]: https://github.com/stdlib-js/stats-base-dists-chi/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/stats-base-dists-chi/main/LICENSE

[chi-distribution]: https://en.wikipedia.org/wiki/Chi_distribution

<!-- <toc-links> -->

[@stdlib/stats/base/dists/chi/ctor]: https://github.com/stdlib-js/stats-base-dists-chi-ctor

[@stdlib/stats/base/dists/chi/entropy]: https://github.com/stdlib-js/stats-base-dists-chi-entropy

[@stdlib/stats/base/dists/chi/kurtosis]: https://github.com/stdlib-js/stats-base-dists-chi-kurtosis

[@stdlib/stats/base/dists/chi/mean]: https://github.com/stdlib-js/stats-base-dists-chi-mean

[@stdlib/stats/base/dists/chi/mode]: https://github.com/stdlib-js/stats-base-dists-chi-mode

[@stdlib/stats/base/dists/chi/skewness]: https://github.com/stdlib-js/stats-base-dists-chi-skewness

[@stdlib/stats/base/dists/chi/stdev]: https://github.com/stdlib-js/stats-base-dists-chi-stdev

[@stdlib/stats/base/dists/chi/variance]: https://github.com/stdlib-js/stats-base-dists-chi-variance

[@stdlib/stats/base/dists/chi/cdf]: https://github.com/stdlib-js/stats-base-dists-chi-cdf

[@stdlib/stats/base/dists/chi/logpdf]: https://github.com/stdlib-js/stats-base-dists-chi-logpdf

[@stdlib/stats/base/dists/chi/pdf]: https://github.com/stdlib-js/stats-base-dists-chi-pdf

[@stdlib/stats/base/dists/chi/quantile]: https://github.com/stdlib-js/stats-base-dists-chi-quantile

<!-- </toc-links> -->

</section>

<!-- /.links -->
