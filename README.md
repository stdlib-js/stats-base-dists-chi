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


<details>
  <summary>
    About stdlib...
  </summary>
  <p>We believe in a future in which the web is a preferred environment for numerical computation. To help realize this future, we've built stdlib. stdlib is a standard library, with an emphasis on numerical and scientific computation, written in JavaScript (and C) for execution in browsers and in Node.js.</p>
  <p>The library is fully decomposable, being architected in such a way that you can swap out and mix and match APIs and functionality to cater to your exact preferences and use cases.</p>
  <p>When you use stdlib, you can be absolutely certain that you are using the most thorough, rigorous, well-written, studied, documented, tested, measured, and high-quality code out there.</p>
  <p>To join us in bringing numerical computing to the web, get started by checking us out on <a href="https://github.com/stdlib-js/stdlib">GitHub</a>, and please consider <a href="https://opencollective.com/stdlib">financially supporting stdlib</a>. We greatly appreciate your continued support!</p>
</details>

# Chi

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Chi distribution.



<section class="usage">

## Usage

```javascript
import chi from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-chi@v0.3.1-deno/mod.js';
```

You can also import the following named exports from the package:

```javascript
import { Chi, cdf, entropy, kurtosis, logpdf, mean, mode, pdf, quantile, skewness, stdev, variance } from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-chi@v0.3.1-deno/mod.js';
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
-   <span class="signature">[`logpdf( x, k )`][@stdlib/stats/base/dists/chi/logpdf]</span><span class="delimiter">: </span><span class="description">evaluate the natural logarithm of the probability density function (PDF) for a chi distribution.</span>
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
var Chi = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-chi' ).Chi;

var dist = new Chi( 4.0 );

var mu = dist.mean;
// returns ~1.88
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
var chiRandomFactory = require( 'https://cdn.jsdelivr.net/gh/stdlib-js/random-base-chi' ).factory;
import filledarrayBy from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-filled-by@deno/mod.js';
import variance from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-strided-variance@deno/mod.js';
import linspace from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-linspace@deno/mod.js';
import rayleigh from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-rayleigh@deno/mod.js';
import absdiff from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-utils-absolute-difference@deno/mod.js';
import mean from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-strided-mean@deno/mod.js';
import abs from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-abs@deno/mod.js';
import max from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-max@deno/mod.js';
import chi from 'https://cdn.jsdelivr.net/gh/stdlib-js/stats-base-dists-chi@v0.3.1-deno/mod.js';

// Define the degrees of freedom parameter:
var k = 2;

// Generate an array of x values:
var x = linspace( 0, 10, 100 );

// Compute the PDF for each x:
var chiPDF = chi.pdf.factory( k );
var pdf = filledarrayBy( x.length, 'float64', chiPDF );

// Compute the CDF for each x:
var chiCDF = chi.cdf.factory( k );
var cdf = filledarrayBy( x.length, 'float64', chiCDF );

// Output the PDF and CDF values:
console.log( 'x values: ', x );
console.log( 'PDF values: ', pdf );
console.log( 'CDF values: ', cdf );

// Compute statistical properties:
var theoreticalMean = chi.mean( k );
var theoreticalVariance = chi.variance( k );
var theoreticalSkewness = chi.skewness( k );
var theoreticalKurtosis = chi.kurtosis( k );

console.log( 'Theoretical Mean: ', theoreticalMean );
console.log( 'Theoretical Variance: ', theoreticalVariance );
console.log( 'Skewness: ', theoreticalSkewness );
console.log( 'Kurtosis: ', theoreticalKurtosis );

// Generate random samples from the Chi distribution:
var rchi = chiRandomFactory( k );
var n = 1000;
var samples = filledarrayBy( n, 'float64', rchi );

// Compute sample mean and variance:
var sampleMean = mean( n, samples, 1 );
var sampleVariance = variance( n, 1, samples, 1 );

console.log( 'Sample Mean: ', sampleMean );
console.log( 'Sample Variance: ', sampleVariance );

// Compare sample statistics to theoretical values:
console.log( 'Difference in Mean: ', abs( theoreticalMean - sampleMean ) );
console.log( 'Difference in Variance: ', abs( theoreticalVariance - sampleVariance ) );

// Demonstrate the relationship with the Rayleigh distribution when k=2:
var rayleighPDF = rayleigh.pdf.factory( 1.0 );
var rayleighCDF = rayleigh.cdf.factory( 1.0 );

// Compute Rayleigh PDF and CDF for each x:
var rayleighPDFValues = filledarrayBy( x.length, 'float64', rayleighPDF );

var rayleighCDFValues = filledarrayBy( x.length, 'float64', rayleighCDF );

// Compare Chi and Rayleigh PDFs and CDFs:
var maxDiffPDF = 0.0;
var maxDiffCDF = 0.0;
var diffPDF;
var diffCDF;
var i;
for ( i = 0; i < x.length; i++ ) {
    diffPDF = absdiff( pdf[ i ], rayleighPDFValues[ i ] );
    maxDiffPDF = max( maxDiffPDF, diffPDF );
    diffCDF = absdiff( cdf[ i ], rayleighCDFValues[ i ] );
    maxDiffCDF = max( maxDiffCDF, diffCDF );
}
console.log( 'Maximum difference between Chi(k=2) PDF and Rayleigh PDF: ', maxDiffPDF );
console.log( 'Maximum difference between Chi(k=2) CDF and Rayleigh CDF: ', maxDiffCDF );
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

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2026. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/stats-base-dists-chi.svg
[npm-url]: https://npmjs.org/package/@stdlib/stats-base-dists-chi

[test-image]: https://github.com/stdlib-js/stats-base-dists-chi/actions/workflows/test.yml/badge.svg?branch=v0.3.1
[test-url]: https://github.com/stdlib-js/stats-base-dists-chi/actions/workflows/test.yml?query=branch:v0.3.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/stats-base-dists-chi/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/stats-base-dists-chi?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/stats-base-dists-chi.svg
[dependencies-url]: https://david-dm.org/stdlib-js/stats-base-dists-chi/main

-->

[chat-image]: https://img.shields.io/badge/zulip-join_chat-brightgreen.svg
[chat-url]: https://stdlib.zulipchat.com

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/stats-base-dists-chi/tree/deno
[deno-readme]: https://github.com/stdlib-js/stats-base-dists-chi/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/stats-base-dists-chi/tree/umd
[umd-readme]: https://github.com/stdlib-js/stats-base-dists-chi/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/stats-base-dists-chi/tree/esm
[esm-readme]: https://github.com/stdlib-js/stats-base-dists-chi/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/stats-base-dists-chi/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/stats-base-dists-chi/main/LICENSE

[chi-distribution]: https://en.wikipedia.org/wiki/Chi_distribution

<!-- <toc-links> -->

[@stdlib/stats/base/dists/chi/ctor]: https://github.com/stdlib-js/stats-base-dists-chi-ctor/tree/deno

[@stdlib/stats/base/dists/chi/entropy]: https://github.com/stdlib-js/stats-base-dists-chi-entropy/tree/deno

[@stdlib/stats/base/dists/chi/kurtosis]: https://github.com/stdlib-js/stats-base-dists-chi-kurtosis/tree/deno

[@stdlib/stats/base/dists/chi/mean]: https://github.com/stdlib-js/stats-base-dists-chi-mean/tree/deno

[@stdlib/stats/base/dists/chi/mode]: https://github.com/stdlib-js/stats-base-dists-chi-mode/tree/deno

[@stdlib/stats/base/dists/chi/skewness]: https://github.com/stdlib-js/stats-base-dists-chi-skewness/tree/deno

[@stdlib/stats/base/dists/chi/stdev]: https://github.com/stdlib-js/stats-base-dists-chi-stdev/tree/deno

[@stdlib/stats/base/dists/chi/variance]: https://github.com/stdlib-js/stats-base-dists-chi-variance/tree/deno

[@stdlib/stats/base/dists/chi/cdf]: https://github.com/stdlib-js/stats-base-dists-chi-cdf/tree/deno

[@stdlib/stats/base/dists/chi/logpdf]: https://github.com/stdlib-js/stats-base-dists-chi-logpdf/tree/deno

[@stdlib/stats/base/dists/chi/pdf]: https://github.com/stdlib-js/stats-base-dists-chi-pdf/tree/deno

[@stdlib/stats/base/dists/chi/quantile]: https://github.com/stdlib-js/stats-base-dists-chi-quantile/tree/deno

<!-- </toc-links> -->

</section>

<!-- /.links -->
