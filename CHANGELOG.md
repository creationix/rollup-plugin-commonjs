# rollup-plugin-commonjs changelog

## 9.2.3
*unreleased*
* Added support for ES3 ancient browsers ([#364](https://github.com/rollup/rollup-plugin-commonjs/issues/364))

## 9.2.2
*2019-03-25*
* Handle array destructuring assignment ([#379](https://github.com/rollup/rollup-plugin-commonjs/issues/379))

## 9.2.1
*2019-02-23*
* Use correct context when manually resolving ids ([#370](https://github.com/rollup/rollup-plugin-commonjs/issues/370))

## 9.2.0
*2018-10-10*
* Fix missing default warning, produce better code when importing known ESM default exports ([#349](https://github.com/rollup/rollup-plugin-commonjs/issues/349))
* Refactor code and add prettier ([#346](https://github.com/rollup/rollup-plugin-commonjs/issues/346))

## 9.1.8
*2018-09-18*
* Ignore virtual modules created by other plugins ([#327](https://github.com/rollup/rollup-plugin-commonjs/issues/327))
* Add "location" and "process" to reserved words ([#330](https://github.com/rollup/rollup-plugin-commonjs/issues/330))

## 9.1.6
*2018-08-24*
* Keep commonJS detection between instantiations ([#338](https://github.com/rollup/rollup-plugin-commonjs/issues/338))

## 9.1.5
*2018-08-09*
* Handle object form of input ([#329](https://github.com/rollup/rollup-plugin-commonjs/issues/329))

## 9.1.4
*2018-07-27*
* Make "from" a reserved word ([#320](https://github.com/rollup/rollup-plugin-commonjs/issues/320))

## 9.1.3
*2018-04-30*
* Fix a caching issue ([#316](https://github.com/rollup/rollup-plugin-commonjs/issues/316))

## 9.1.2
*2018-04-30*
* Re-publication of 9.1.0

## 9.1.1
*2018-04-30*
* Fix ordering of modules when using rollup 0.58 ([#302](https://github.com/rollup/rollup-plugin-commonjs/issues/302))

## 9.1.0

* Do not automatically wrap modules with return statements in top level arrow functions ([#302](https://github.com/rollup/rollup-plugin-commonjs/issues/302))

## 9.0.0

* Make rollup a peer dependency with a version range ([#300](https://github.com/rollup/rollup-plugin-commonjs/issues/300))

## 8.4.1

* Re-release of 8.3.0 as #287 was actually a breaking change

## 8.4.0

* Better handle non-CJS files that contain CJS keywords ([#285](https://github.com/rollup/rollup-plugin-commonjs/issues/285))
* Use rollup's plugin context`parse` function ([#287](https://github.com/rollup/rollup-plugin-commonjs/issues/287))
* Improve error handling ([#288](https://github.com/rollup/rollup-plugin-commonjs/issues/288))

## 8.3.0

* Handle multiple entry points ([#283](https://github.com/rollup/rollup-plugin-commonjs/issues/283))
* Extract named exports from exported object literals ([#272](https://github.com/rollup/rollup-plugin-commonjs/issues/272))
* Fix when `options.external` is modified by other plugins ([#264](https://github.com/rollup/rollup-plugin-commonjs/issues/264))
* Recognize static template strings in require statements ([#271](https://github.com/rollup/rollup-plugin-commonjs/issues/271))

## 8.2.4

* Don't import default from ES modules that don't export default ([#206](https://github.com/rollup/rollup-plugin-commonjs/issues/206))

## 8.2.3

* Prevent duplicate default exports ([#230](https://github.com/rollup/rollup-plugin-commonjs/pull/230))
* Only include default export when it exists ([#226](https://github.com/rollup/rollup-plugin-commonjs/pull/226))
* Deconflict `require` aliases ([#232](https://github.com/rollup/rollup-plugin-commonjs/issues/232))

## 8.2.1

* Fix magic-string deprecation warning

## 8.2.0

* Avoid using `index` as a variable name ([#208](https://github.com/rollup/rollup-plugin-commonjs/pull/208))

## 8.1.1

* Compatibility with 0.48 ([#220](https://github.com/rollup/rollup-plugin-commonjs/issues/220))

## 8.1.0

* Handle `options.external` correctly ([#212](https://github.com/rollup/rollup-plugin-commonjs/pull/212))
* Support top-level return ([#195](https://github.com/rollup/rollup-plugin-commonjs/pull/195))

## 8.0.2

* Fix another `var` rewrite bug ([#181](https://github.com/rollup/rollup-plugin-commonjs/issues/181))

## 8.0.1

* Remove declarators within a var declaration correctly ([#179](https://github.com/rollup/rollup-plugin-commonjs/issues/179))

## 8.0.0

* Prefer the names dependencies are imported by for the common `var foo = require('foo')` pattern ([#176](https://github.com/rollup/rollup-plugin-commonjs/issues/176))

## 7.1.0

* Allow certain `require` statements to pass through unmolested ([#174](https://github.com/rollup/rollup-plugin-commonjs/issues/174))

## 7.0.2

* Handle duplicate default exports ([#158](https://github.com/rollup/rollup-plugin-commonjs/issues/158))

## 7.0.1

* Fix exports with parentheses ([#168](https://github.com/rollup/rollup-plugin-commonjs/issues/168))

## 7.0.0

* Rewrite `typeof module`, `typeof module.exports` and `typeof exports` as `'object'` ([#151](https://github.com/rollup/rollup-plugin-commonjs/issues/151))

## 6.0.1

* Don't overwrite globals ([#127](https://github.com/rollup/rollup-plugin-commonjs/issues/127))

## 6.0.0

* Rewrite top-level `define` as `undefined`, so AMD-first UMD blocks do not cause breakage ([#144](https://github.com/rollup/rollup-plugin-commonjs/issues/144))
* Support ES2017 syntax ([#132](https://github.com/rollup/rollup-plugin-commonjs/issues/132))
* Deconflict exported reserved keywords ([#116](https://github.com/rollup/rollup-plugin-commonjs/issues/116))

## 5.0.5
* Fix parenthesis wrapped exports ([#120](https://github.com/rollup/rollup-plugin-commonjs/issues/120))

## 5.0.4

* Ensure named exports are added to default export in optimised modules ([#112](https://github.com/rollup/rollup-plugin-commonjs/issues/112))

## 5.0.3

* Respect custom `namedExports` in optimised modules ([#35](https://github.com/rollup/rollup-plugin-commonjs/issues/35))

## 5.0.2

* Replace `require` (outside call expressions) with `commonjsRequire` helper ([#77](https://github.com/rollup/rollup-plugin-commonjs/issues/77), [#83](https://github.com/rollup/rollup-plugin-commonjs/issues/83))

## 5.0.1

* Deconflict against globals ([#84](https://github.com/rollup/rollup-plugin-commonjs/issues/84))

## 5.0.0

* Optimise modules that don't need to be wrapped in a function ([#106](https://github.com/rollup/rollup-plugin-commonjs/pull/106))
* Ignore modules containing `import` and `export` statements ([#96](https://github.com/rollup/rollup-plugin-commonjs/pull/96))

## 4.1.0

* Ignore dead branches ([#93](https://github.com/rollup/rollup-plugin-commonjs/issues/93))

## 4.0.1

* Fix `ignoreGlobal` option ([#86](https://github.com/rollup/rollup-plugin-commonjs/pull/86))

## 4.0.0

* Better interop and smaller output ([#92](https://github.com/rollup/rollup-plugin-commonjs/pull/92))

## 3.3.1

* Deconflict export and local module ([rollup/rollup#554](https://github.com/rollup/rollup/issues/554))

## 3.3.0

* Keep the order of execution for require calls ([#43](https://github.com/rollup/rollup-plugin-commonjs/pull/43))
* Use interopDefault as helper ([#42](https://github.com/rollup/rollup-plugin-commonjs/issues/42))

## 3.2.0

* Use named exports as a function when no default export is defined ([#524](https://github.com/rollup/rollup/issues/524))

## 3.1.0

* Replace `typeof require` with `'function'` ([#38](https://github.com/rollup/rollup-plugin-commonjs/issues/38))
* Don't attempt to resolve entry file relative to importer ([#63](https://github.com/rollup/rollup-plugin-commonjs/issues/63))

## 3.0.2

* Handle multiple references to `global`

## 3.0.1

* Return a `name`

## 3.0.0

* Make `transform` stateless ([#71](https://github.com/rollup/rollup-plugin-commonjs/pull/71))
* Support web worker `global` ([#50](https://github.com/rollup/rollup-plugin-commonjs/issues/50))
* Ignore global with `options.ignoreGlobal` ([#48](https://github.com/rollup/rollup-plugin-commonjs/issues/48))

## 2.2.1

* Prevent false positives with `namedExports` ([#36](https://github.com/rollup/rollup-plugin-commonjs/issues/36))

## 2.2.0

* Rewrite top-level `this` expressions to mean the same as `global`  ([#31](https://github.com/rollup/rollup-plugin-commonjs/issues/31))

## 2.1.0

* Optimised module wrappers ([#20](https://github.com/rollup/rollup-plugin-commonjs/pull/20))
* Allow control over named exports via `options.namedExports` ([#18](https://github.com/rollup/rollup-plugin-commonjs/issues/18))
* Handle bare imports correctly ([#23](https://github.com/rollup/rollup-plugin-commonjs/issues/23))
* Blacklist all reserved words as export names ([#21](https://github.com/rollup/rollup-plugin-commonjs/issues/21))
* Configure allowed file extensions via `options.extensions` ([#27](https://github.com/rollup/rollup-plugin-commonjs/pull/27))

## 2.0.0

* Support for transpiled modules – `exports.default` is used as the default export in place of `module.exports`, if applicable, and `__esModule` is not exported ([#16](https://github.com/rollup/rollup-plugin-commonjs/pull/16))

## 1.4.0

* Generate sourcemaps by default

## 1.3.0

* Handle references to `global` ([#6](https://github.com/rollup/rollup-plugin-commonjs/issues/6))

## 1.2.0

* Generate named exports where possible ([#5](https://github.com/rollup/rollup-plugin-commonjs/issues/5))
* Handle shadowed `require`/`module`/`exports`

## 1.1.0

* Handle dots in filenames ([#3](https://github.com/rollup/rollup-plugin-commonjs/issues/3))
* Wrap modules in IIFE for more readable output

## 1.0.0

* Stable release, now that Rollup supports plugins

## 0.2.1

* Allow mixed CommonJS/ES6 imports/exports
* Use `var` instead of `let`

## 0.2.0

* Sourcemap support
* Support `options.include` and `options.exclude`
* Bail early if module is obviously not a CommonJS module

## 0.1.1

Add dist files to package (whoops!)

## 0.1.0

* First release
