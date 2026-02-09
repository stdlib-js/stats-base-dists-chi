# CHANGELOG

> Package changelog.

<section class="release" id="v0.3.1">

## 0.3.1 (2026-02-08)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.3.0">

## 0.3.0 (2026-01-30)

<section class="features">

### Features

-   [`3109ba5`](https://github.com/stdlib-js/stdlib/commit/3109ba5061cbdfd2c95258aafc8bf42884e6691c) - add C implementation for `stats/base/dists/chi/cdf`
-   [`6cfd0be`](https://github.com/stdlib-js/stdlib/commit/6cfd0be5c0bc3fa6dcf23629975a7971f4bbb776) - add C implementation for `stats/base/dists/chi/kurtosis`
-   [`26936b8`](https://github.com/stdlib-js/stdlib/commit/26936b8c598cb1461ca4a6b6a237db95b16605b1) - add C implementation for `stats/base/dists/chi/skewness`
-   [`a79528c`](https://github.com/stdlib-js/stdlib/commit/a79528cdc868d7ad54312192e561288503793b0b) - add C implementation for `stats/base/dists/chi/logpdf` [(#4527)](https://github.com/stdlib-js/stdlib/pull/4527)
-   [`b02b1dc`](https://github.com/stdlib-js/stdlib/commit/b02b1dcda79311b83e803051d3f396f2b3d43874) - add C implementation for `stats/base/dists/chi/pdf` [(#4526)](https://github.com/stdlib-js/stdlib/pull/4526)
-   [`053722e`](https://github.com/stdlib-js/stdlib/commit/053722e28d6b086a08fc017948ae364976d9601c) - **stats:** add C implementation for `stats/base/dists/chi/stdev` [(#4590)](https://github.com/stdlib-js/stdlib/pull/4590)
-   [`8b7ddc2`](https://github.com/stdlib-js/stdlib/commit/8b7ddc2cdc3dd40b27d7ef9f2a2a5729a4f5c3aa) - **stats:** add C implementation for `stats/base/dists/chi/variance` [(#4591)](https://github.com/stdlib-js/stdlib/pull/4591)
-   [`9e43626`](https://github.com/stdlib-js/stdlib/commit/9e436263a3b0cf8c54da48f9c73cc94826baa57e) - add C implementation for `stats/base/dists/chi/mean` [(#4514)](https://github.com/stdlib-js/stdlib/pull/4514)
-   [`26f2135`](https://github.com/stdlib-js/stdlib/commit/26f2135d154546c9ba01536c23cedd736cf607fc) - add C implementation for `stats/base/dists/chi/entropy` [(#4589)](https://github.com/stdlib-js/stdlib/pull/4589)
-   [`a6f8779`](https://github.com/stdlib-js/stdlib/commit/a6f8779298b6200a63ad80f40e6769bdf3ccc58d) - add C implementation for `stats/base/dists/chi/mode` [(#3965)](https://github.com/stdlib-js/stdlib/pull/3965)

</section>

<!-- /.features -->

<section class="bug-fixes">

### Bug Fixes

-   [`1a48ebb`](https://github.com/stdlib-js/stdlib/commit/1a48ebbacff02aa8f374081b3b636bc2c0a027ef) - use correct Makefile for examples/c

</section>

<!-- /.bug-fixes -->

<section class="issues">

### Closed Issues

A total of 8 issues were closed in this release:

[#3490](https://github.com/stdlib-js/stdlib/issues/3490), [#3492](https://github.com/stdlib-js/stdlib/issues/3492), [#3493](https://github.com/stdlib-js/stdlib/issues/3493), [#3494](https://github.com/stdlib-js/stdlib/issues/3494), [#3495](https://github.com/stdlib-js/stdlib/issues/3495), [#3498](https://github.com/stdlib-js/stdlib/issues/3498), [#3499](https://github.com/stdlib-js/stdlib/issues/3499), [#7415](https://github.com/stdlib-js/stdlib/issues/7415)

</section>

<!-- /.issues -->

<section class="commits">

### Commits

<details>

-   [`a27671f`](https://github.com/stdlib-js/stdlib/commit/a27671f8fc907e4f054086e3e422234ed56964cd) - **docs:** update string interpolation in various `stats/base/dists` examples [(#9533)](https://github.com/stdlib-js/stdlib/pull/9533) _(by Harsh Yadav)_
-   [`88fe77a`](https://github.com/stdlib-js/stdlib/commit/88fe77a2f059149b803f51d1a787894c7670798b) - **docs:** fix example code in namespace TypeScript declarations _(by Philipp Burckhardt)_
-   [`9b13062`](https://github.com/stdlib-js/stdlib/commit/9b130625f0f19866a877023e9be85204636ef01e) - **docs:** fix return values in TSDoc return annotation comments _(by Philipp Burckhardt)_
-   [`2cabe18`](https://github.com/stdlib-js/stdlib/commit/2cabe1887e6a502a306b70580fb5d038da0917f3) - **docs:** fix return values in TSDoc return annotation comments _(by Philipp Burckhardt)_
-   [`e2efe32`](https://github.com/stdlib-js/stdlib/commit/e2efe32914d0d9dae5da34e6f7e7bf7655430710) - **chore:** rename exported variable in d.ts file to match name used in example code _(by Philipp Burckhardt)_
-   [`e678757`](https://github.com/stdlib-js/stdlib/commit/e678757c9a62631a907278ec13a5d7b27c0f1e15) - **docs:** fix return annotation values _(by Philipp Burckhardt)_
-   [`7add020`](https://github.com/stdlib-js/stdlib/commit/7add0201c13e56a0381926ccfd4073c84eaf2ed4) - **test:** use standardized assertion messages and fix lint errors _(by Philipp Burckhardt)_
-   [`fc438e0`](https://github.com/stdlib-js/stdlib/commit/fc438e0edbad0689d6923d6f3edb959b96597662) - **test:** use standardized assertion messages and fix lint errors _(by Philipp Burckhardt)_
-   [`07f7c05`](https://github.com/stdlib-js/stdlib/commit/07f7c0522c73e6ad9505e1d45035ae439344200d) - **test:** use standardized assertion messages and fix lint errors _(by Philipp Burckhardt)_
-   [`9c21fd2`](https://github.com/stdlib-js/stdlib/commit/9c21fd20ef8b8a6a88abb96d80ea6d8e4c5434eb) - **test:** use .strictEqual() instead of .equal() _(by Philipp Burckhardt)_
-   [`8ea46b6`](https://github.com/stdlib-js/stdlib/commit/8ea46b662dc6e27231d250d101e33a3cf770cd77) - **test:** update descriptions to match language used in JS tests _(by Philipp Burckhardt)_
-   [`e342a38`](https://github.com/stdlib-js/stdlib/commit/e342a388619ab71f5222105ec94c5029e42a4458) - **refactor:** update paths _(by Gururaj Gurram)_
-   [`a4ce77e`](https://github.com/stdlib-js/stdlib/commit/a4ce77efe910c9398e75b767fb81e786a3a04cc0) - **test:** pass in opts to skip if addon is not available _(by Philipp Burckhardt)_
-   [`1a48ebb`](https://github.com/stdlib-js/stdlib/commit/1a48ebbacff02aa8f374081b3b636bc2c0a027ef) - **fix:** use correct Makefile for examples/c _(by Philipp Burckhardt)_
-   [`3109ba5`](https://github.com/stdlib-js/stdlib/commit/3109ba5061cbdfd2c95258aafc8bf42884e6691c) - **feat:** add C implementation for `stats/base/dists/chi/cdf` _(by Philipp Burckhardt)_
-   [`6cfd0be`](https://github.com/stdlib-js/stdlib/commit/6cfd0be5c0bc3fa6dcf23629975a7971f4bbb776) - **feat:** add C implementation for `stats/base/dists/chi/kurtosis` _(by Philipp Burckhardt)_
-   [`26936b8`](https://github.com/stdlib-js/stdlib/commit/26936b8c598cb1461ca4a6b6a237db95b16605b1) - **feat:** add C implementation for `stats/base/dists/chi/skewness` _(by Philipp Burckhardt)_
-   [`a4464fb`](https://github.com/stdlib-js/stdlib/commit/a4464fbc05304fd3607b4c0471734a239b5451cb) - **chore:** address commit comments for commit `b02b1dc` [(#7423)](https://github.com/stdlib-js/stdlib/pull/7423) _(by Lokesh Ranjan)_
-   [`354a54b`](https://github.com/stdlib-js/stdlib/commit/354a54b69858eae98fb4b757d72ca3dde5ec1f4a) - **test:** match tolerance used for JS implementation _(by Philipp Burckhardt)_
-   [`a79528c`](https://github.com/stdlib-js/stdlib/commit/a79528cdc868d7ad54312192e561288503793b0b) - **feat:** add C implementation for `stats/base/dists/chi/logpdf` [(#4527)](https://github.com/stdlib-js/stdlib/pull/4527) _(by Aadish Jain, Philipp Burckhardt, stdlib-bot)_
-   [`b02b1dc`](https://github.com/stdlib-js/stdlib/commit/b02b1dcda79311b83e803051d3f396f2b3d43874) - **feat:** add C implementation for `stats/base/dists/chi/pdf` [(#4526)](https://github.com/stdlib-js/stdlib/pull/4526) _(by Aadish Jain, Philipp Burckhardt, stdlib-bot)_
-   [`3565318`](https://github.com/stdlib-js/stdlib/commit/3565318e3639b3e44890ed15ccd73560d3cac14c) - **refactor:** update paths _(by Gururaj Gurram)_
-   [`20dd4e8`](https://github.com/stdlib-js/stdlib/commit/20dd4e891d7fac27581eecb54240ae194d6076ab) - **test:** add missing skips for native add-on tests _(by Philipp Burckhardt)_
-   [`b51a457`](https://github.com/stdlib-js/stdlib/commit/b51a457474fb3527c628001639fc4e1174ed45e4) - **bench:** update random value generation [(#7010)](https://github.com/stdlib-js/stdlib/pull/7010) _(by Harsh Yadav)_
-   [`876d319`](https://github.com/stdlib-js/stdlib/commit/876d319235fa6b11ff7df92a34f3ebba821d6630) - **bench:** update random value generation [(#7009)](https://github.com/stdlib-js/stdlib/pull/7009) _(by Harsh Yadav)_
-   [`7788818`](https://github.com/stdlib-js/stdlib/commit/77888181398b4aa628194b37b058e262c8bdb7fd) - **docs:** replace manual `for` loop in examples [(#6921)](https://github.com/stdlib-js/stdlib/pull/6921) _(by Harsh Yadav)_
-   [`828cfd5`](https://github.com/stdlib-js/stdlib/commit/828cfd594d771e9d1ba2af3e80af0021f0b7fd8f) - **docs:** replace manual `for` loop in examples [(#6922)](https://github.com/stdlib-js/stdlib/pull/6922) _(by Harsh Yadav)_
-   [`053722e`](https://github.com/stdlib-js/stdlib/commit/053722e28d6b086a08fc017948ae364976d9601c) - **feat(stats):** add C implementation for `stats/base/dists/chi/stdev` [(#4590)](https://github.com/stdlib-js/stdlib/pull/4590) _(by Karan Anand, Philipp Burckhardt, stdlib-bot)_
-   [`8b7ddc2`](https://github.com/stdlib-js/stdlib/commit/8b7ddc2cdc3dd40b27d7ef9f2a2a5729a4f5c3aa) - **feat(stats):** add C implementation for `stats/base/dists/chi/variance` [(#4591)](https://github.com/stdlib-js/stdlib/pull/4591) _(by Karan Anand, Philipp Burckhardt, stdlib-bot)_
-   [`9e43626`](https://github.com/stdlib-js/stdlib/commit/9e436263a3b0cf8c54da48f9c73cc94826baa57e) - **feat:** add C implementation for `stats/base/dists/chi/mean` [(#4514)](https://github.com/stdlib-js/stdlib/pull/4514) _(by Aadish Jain, Philipp Burckhardt, stdlib-bot)_
-   [`23c60da`](https://github.com/stdlib-js/stdlib/commit/23c60daf037b609ab1315f45448e0ba52a89c247) - **docs:** remove spaces before periods _(by Philipp Burckhardt)_
-   [`a1e230f`](https://github.com/stdlib-js/stdlib/commit/a1e230f29297caa89880e9c194c615a0400fb7bc) - **chore:** clean up cppcheck-suppress comments _(by Karan Anand)_
-   [`f7988d3`](https://github.com/stdlib-js/stdlib/commit/f7988d3c02e0eff3bd9bd7523b5dc975bb98dc0e) - **bench:** fix `isnan` checks in `stats/base/dists` [(#5296)](https://github.com/stdlib-js/stdlib/pull/5296) _(by Karan Anand)_
-   [`911e179`](https://github.com/stdlib-js/stdlib/commit/911e1793885aced96a177f2ea54300503b2c2a26) - **docs:** clean-up of C docstrings _(by Philipp Burckhardt)_
-   [`e61b1de`](https://github.com/stdlib-js/stdlib/commit/e61b1dee3334bacf30d213de5b5f1c7868c0753b) - **docs:** clean-up of C docstrings _(by Philipp Burckhardt)_
-   [`26f2135`](https://github.com/stdlib-js/stdlib/commit/26f2135d154546c9ba01536c23cedd736cf607fc) - **feat:** add C implementation for `stats/base/dists/chi/entropy` [(#4589)](https://github.com/stdlib-js/stdlib/pull/4589) _(by Karan Anand, Philipp Burckhardt, stdlib-bot)_
-   [`b3540a8`](https://github.com/stdlib-js/stdlib/commit/b3540a8ffa4c9cd3122e660a68dcbe286330b5e6) - **bench:** refactor random number generation in `stats/base/dists/chi` [(#4853)](https://github.com/stdlib-js/stdlib/pull/4853) _(by Karan Anand)_
-   [`177f0a0`](https://github.com/stdlib-js/stdlib/commit/177f0a00909c097be05d47107a3e6ab05b865409) - **chore:** consistently use differential entropy for continuous distributions _(by Philipp Burckhardt)_
-   [`f75a0ce`](https://github.com/stdlib-js/stdlib/commit/f75a0cef6a3112b166dba04c13bada9763cec350) - **chore:** use excess kurtosis consistently _(by Philipp Burckhardt)_
-   [`998c1be`](https://github.com/stdlib-js/stdlib/commit/998c1be8630c1efcf19beefda88181db820d1dcb) - **chore:** remove EPS addition and directly draw from desired distribution _(by Philipp Burckhardt)_
-   [`8bf8285`](https://github.com/stdlib-js/stdlib/commit/8bf8285aba0ecbd00ae145c4c5c098cd28135814) - **chore:** minor clean-up _(by Philipp Burckhardt)_
-   [`a6f8779`](https://github.com/stdlib-js/stdlib/commit/a6f8779298b6200a63ad80f40e6769bdf3ccc58d) - **feat:** add C implementation for `stats/base/dists/chi/mode` [(#3965)](https://github.com/stdlib-js/stdlib/pull/3965) _(by Vivek Maurya, Philipp Burckhardt)_
-   [`43e7a33`](https://github.com/stdlib-js/stdlib/commit/43e7a3386606e54475e872d24ddf11fa6c122c42) - **chore:** minor clean-up after code review _(by Philipp Burckhardt)_
-   [`f0ab00b`](https://github.com/stdlib-js/stdlib/commit/f0ab00bf081e55b928de80320c75dc42e713ad3d) - **docs:** improve README examples of `stats/base/dists/chi` namespace [(#1803)](https://github.com/stdlib-js/stdlib/pull/1803) _(by Shivam Ahir, Philipp Burckhardt)_

</details>

</section>

<!-- /.commits -->

<section class="contributors">

### Contributors

A total of 8 people contributed to this release. Thank you to the following contributors:

-   Aadish Jain
-   Gururaj Gurram
-   Harsh Yadav
-   Karan Anand
-   Lokesh Ranjan
-   Philipp Burckhardt
-   Shivam Ahir
-   Vivek Maurya

</section>

<!-- /.contributors -->

</section>

<!-- /.release -->

<section class="release" id="v0.2.2">

## 0.2.2 (2024-07-28)

<section class="commits">

### Commits

<details>

-   [`41d41e9`](https://github.com/stdlib-js/stdlib/commit/41d41e959b4eaad3c631e6898e3144a4015a5458) - **test:** include trailing newlines in Julia-generated JSON fixtures _(by Philipp Burckhardt)_
-   [`9ed7d0e`](https://github.com/stdlib-js/stdlib/commit/9ed7d0e7d57edb5ad0dfb65c944bed87d475cbf3) - **chore:** add missing trailing newlines _(by Philipp Burckhardt)_

</details>

</section>

<!-- /.commits -->

<section class="contributors">

### Contributors

A total of 1 person contributed to this release. Thank you to this contributor:

-   Philipp Burckhardt

</section>

<!-- /.contributors -->

</section>

<!-- /.release -->

<section class="release" id="v0.2.1">

## 0.2.1 (2024-02-24)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.2.0">

## 0.2.0 (2024-02-14)

<section class="commits">

### Commits

<details>

-   [`9502ed2`](https://github.com/stdlib-js/stdlib/commit/9502ed27e2853e312c556a48bdd7775095e66709) - **build:** replace tslint directive with eslint equivalent _(by Philipp Burckhardt)_
-   [`d73bbf4`](https://github.com/stdlib-js/stdlib/commit/d73bbf43d222f935085f8ecf7526e5f57835f74e) - **build:** replace lint directives _(by Philipp Burckhardt)_

</details>

</section>

<!-- /.commits -->

<section class="contributors">

### Contributors

A total of 1 person contributed to this release. Thank you to this contributor:

-   Philipp Burckhardt

</section>

<!-- /.contributors -->

</section>

<!-- /.release -->

<section class="release" id="v0.1.0">

## 0.1.0 (2023-09-24)

<section class="features">

### Features

-   [`81ca3ab`](https://github.com/stdlib-js/stdlib/commit/81ca3ab33585150e98a402b3e6d57beb1ec36864) - update minimum TypeScript version

</section>

<!-- /.features -->

<section class="breaking-changes">

### BREAKING CHANGES

-   [`81ca3ab`](https://github.com/stdlib-js/stdlib/commit/81ca3ab33585150e98a402b3e6d57beb1ec36864): update minimum TypeScript version to 4.1

    -   To migrate, users should upgrade their TypeScript version to at least version 4.1.

</section>

<!-- /.breaking-changes -->

<section class="commits">

### Commits

<details>

-   [`81ca3ab`](https://github.com/stdlib-js/stdlib/commit/81ca3ab33585150e98a402b3e6d57beb1ec36864) - **feat:** update minimum TypeScript version _(by Philipp Burckhardt)_
-   [`d5fa8e8`](https://github.com/stdlib-js/stdlib/commit/d5fa8e8a6267a837a25a7027e9fe3e847bc2d1c5) - **test:** use strictEqual checks _(by Philipp Burckhardt)_
-   [`ce7e336`](https://github.com/stdlib-js/stdlib/commit/ce7e3367c0f9477773fe76dd0eca64dc6ad33c02) - **docs:** update equations _(by Philipp Burckhardt)_
-   [`37f032d`](https://github.com/stdlib-js/stdlib/commit/37f032d4a571f667ea99f6f52f60b5d736c627f3) - **docs:** render equations via math code blocks _(by Philipp Burckhardt)_

</details>

</section>

<!-- /.commits -->

<section class="contributors">

### Contributors

A total of 1 person contributed to this release. Thank you to this contributor:

-   Philipp Burckhardt

</section>

<!-- /.contributors -->

</section>

<!-- /.release -->

<section class="release" id="v0.0.7">

## 0.0.7 (2022-07-08)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.0.6">

## 0.0.6 (2022-02-16)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.0.5">

## 0.0.5 (2021-08-22)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.0.4">

## 0.0.4 (2021-07-07)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.0.3">

## 0.0.3 (2021-06-27)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.0.2">

## 0.0.2 (2021-06-16)

No changes reported for this release.

</section>

<!-- /.release -->

<section class="release" id="v0.0.1">

## 0.0.1 (2021-06-15)

No changes reported for this release.

</section>

<!-- /.release -->

