<!--

@license Apache-2.0

Copyright (c) 2026 The Stdlib Authors.

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

# Uint64

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Unsigned 64-bit integer.

<!-- Section to include introductory text. Make sure to keep an empty line after the intro `section` element and another before the `/section` close. -->

<section class="intro">

</section>

<!-- /.intro -->

<!-- Package usage documentation. -->



<section class="usage">

## Usage

```javascript
import Uint64 from 'https://cdn.jsdelivr.net/gh/stdlib-js/number-uint64-ctor@esm/index.mjs';
```

#### Uint64( value )

Unsigned 64-bit integer constructor.

```javascript
var x = new Uint64( 5 );
// returns <Uint64>
```

* * *

## Properties

#### Uint64.name

Static property returning the constructor name.

```javascript
var str = Uint64.name;
// returns 'Uint64'
```

#### Uint64.BYTES_PER_ELEMENT

Size (in bytes) of the underlying value.

```javascript
var nbytes = Uint64.BYTES_PER_ELEMENT;
// returns 8
```

#### Uint64.prototype.BYTES_PER_ELEMENT

Size (in bytes) of the underlying value.

```javascript
var x = new Uint64( 5 );

var nbytes = x.BYTES_PER_ELEMENT;
// returns 8
```

#### Uint64.prototype.byteLength

Size (in bytes) of the underlying value.

```javascript
var x = new Uint64( 5 );

var nbytes = x.byteLength;
// returns 8
```

#### Uint64.prototype.hi

High 32-bit word of an unsigned 64-bit integer.

```javascript
var x = Uint64.from( [ 1234, 5678 ] );

var w = x.hi;
// returns 1234
```

#### Uint64.prototype.lo

Low 32-bit word of an unsigned 64-bit integer.

```javascript
var x = Uint64.from( [ 1234, 5678 ] );

var w = x.lo;
// returns 5678
```

* * *

## Methods

### Static Methods

#### Uint64.from( array )

Creates a new unsigned 64-bit integer from an array-like object containing a high and low word.

```javascript
var x = Uint64.from( [ 1234, 5678 ] );
// returns <Uint64>
```

#### Uint64.of( high, low )

Creates a new unsigned 64-bit integer from a high and low word.

```javascript
var x = Uint64.of( 1234, 5678 );
// returns <Uint64>
```

### Accessor Methods

These methods do **not** mutate a `Uint64` instance and, instead, return an unsigned 64-bit integer representation.

#### Uint64.prototype.toString()

Returns a string representation of a `Uint64` instance.

```javascript
var x = new Uint64( 5 );
var str = x.toString();
// returns '5'
```

#### Uint64.prototype.toJSON()

Returns a [JSON][json] representation of a `Uint64` instance. [`JSON.stringify()`][mdn-json-stringify] implicitly calls this method when stringifying a `Uint64` instance.

```javascript
var x = new Uint64( 5 );

var o = x.toJSON();
// returns { 'type': 'Uint64', 'words': [ 0, 5 ] }
```

To [revive][mdn-json-parse] a `Uint64` instance from a [JSON][json] string, see [@stdlib/number/uint64/reviver][@stdlib/number/uint64/reviver].

#### Uint64.prototype.valueOf()

Converts a `Uint64` instance to a primitive value.

```javascript
var x = new Uint64( 5 );

var v = x.valueOf();
// e.g., returns <bigint>
```

</section>

<!-- /.usage -->

* * *

<!-- Package usage notes. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="notes">

## Notes

-   An unsigned 64-bit integer has a range of \[`0`, `2^64-1`\].

</section>

<!-- /.notes -->

* * *

<!-- Package usage examples. -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```html
<!DOCTYPE html>
<html lang="en">
<body>
<script type="module">

import Uint64 from 'https://cdn.jsdelivr.net/gh/stdlib-js/number-uint64-ctor@esm/index.mjs';

var x = new Uint64( 1234 );

console.log( 'type: %s', typeof x );
// => 'type: object'

console.log( 'str: %s', x );
// => 'str: 1234'

console.log( 'JSON: %s', JSON.stringify( x ) );
// => 'JSON: {"type":"Uint64","words":[0,1234]}'

</script>
</body>
</html>
```

</section>

<!-- /.examples -->


<!-- Section to include cited references. If references are included, add a horizontal rule *before* the section. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="references">

</section>

<!-- /.references -->

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/number-uint64-ctor.svg
[npm-url]: https://npmjs.org/package/@stdlib/number-uint64-ctor

[test-image]: https://github.com/stdlib-js/number-uint64-ctor/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/number-uint64-ctor/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/number-uint64-ctor/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/number-uint64-ctor?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/number-uint64-ctor.svg
[dependencies-url]: https://david-dm.org/stdlib-js/number-uint64-ctor/main

-->

[chat-image]: https://img.shields.io/badge/zulip-join_chat-brightgreen.svg
[chat-url]: https://stdlib.zulipchat.com

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/number-uint64-ctor/tree/deno
[deno-readme]: https://github.com/stdlib-js/number-uint64-ctor/blob/deno/README.md
[umd-url]: https://github.com/stdlib-js/number-uint64-ctor/tree/umd
[umd-readme]: https://github.com/stdlib-js/number-uint64-ctor/blob/umd/README.md
[esm-url]: https://github.com/stdlib-js/number-uint64-ctor/tree/esm
[esm-readme]: https://github.com/stdlib-js/number-uint64-ctor/blob/esm/README.md
[branches-url]: https://github.com/stdlib-js/number-uint64-ctor/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/number-uint64-ctor/main/LICENSE

[json]: http://www.json.org/

[mdn-json-stringify]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/stringify

[mdn-json-parse]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/JSON/parse

[@stdlib/number/uint64/reviver]: https://github.com/stdlib-js/number-uint64-reviver/tree/esm

<!-- <related-links> -->

<!-- </related-links> -->

</section>

<!-- /.links -->
