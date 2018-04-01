# Make Error Cause

[![NPM version][npm-image]][npm-url]
[![NPM downloads][downloads-image]][downloads-url]
[![Build status][travis-image]][travis-url]
[![Test coverage][coveralls-image]][coveralls-url]

> Make your own nested errors.

## Features

* Compatible with node.js and browsers
* Works with `instanceof`
* Output full cause with `err.fullStack`
* Extends [`make-error`](https://github.com/JsCommunity/make-error)

## Installation

```
npm install make-error-cause --save
```

## Usage

```js
import { BaseError } from 'make-error-cause'

class CustomError extends BaseError {
  constructor (message, cause) {
    super(message, cause)
  }
}
```

## Attribution

Inspired by [`verror`](https://www.npmjs.com/package/verror), and others, but created lighter and without core dependencies for browser usage.

Other references:

* [Java](https://docs.oracle.com/javase/7/docs/api/java/lang/Exception.html)
* [Python](https://www.python.org/dev/peps/pep-3134/)

## License

Apache 2.0

[npm-image]: https://img.shields.io/npm/v/make-error-cause.svg?style=flat
[npm-url]: https://npmjs.org/package/make-error-cause
[downloads-image]: https://img.shields.io/npm/dm/make-error-cause.svg?style=flat
[downloads-url]: https://npmjs.org/package/make-error-cause
[travis-image]: https://img.shields.io/travis/blakeembrey/make-error-cause.svg?style=flat
[travis-url]: https://travis-ci.org/blakeembrey/make-error-cause
[coveralls-image]: https://img.shields.io/coveralls/blakeembrey/make-error-cause.svg?style=flat
[coveralls-url]: https://coveralls.io/r/blakeembrey/make-error-cause?branch=master
