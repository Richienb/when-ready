# Whenever ready [![Travis CI Build Status](https://img.shields.io/travis/com/Richienb/whenever-ready/master.svg?style=for-the-badge)](https://travis-ci.com/Richienb/whenever-ready)

A promise that resolves when a value is set.

[![NPM Badge](https://nodei.co/npm/whenever-ready.png)](https://npmjs.com/package/whenever-ready)

## Install

```sh
npm install whenever-ready
```

## Usage

```js
const WheneverReady = require("whenever-ready");
const wReady = new WheneverReady();

wReady.when().then(() => console.log("READY!")); // Listen for readiness.
wReady.ready = true; // Set as ready.
```

## API

### `class` WheneverReady(ready?)

#### ready

Type: `boolean`\
Default: `false`

The initial readiness value.

### `instance` WheneverReady

#### ready

Type: `boolean`\
Default: `false`

The readiness.

#### when()

Returns: `Promise`

Returns a promise that will resolve when `ready` is true.
