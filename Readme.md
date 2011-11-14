# urun

[![Build Status](https://secure.travis-ci.org/felixge/node-urun.png)](http://travis-ci.org/felixge/node-urun)

The minimal test runner.

## Why yet another test runner?

I wanted something simple, that just runs test files, shows progress, and
behaves like a good UNIX citizen. Now it exists.

## Install

```
npm install urun
```

## Usage

In order to execute all test-*.js files inside a given directory, simply do:

```js
require('urun')(__dirname);
```

You now get a nice progress indication, as well as detailed output for each
test that fails.

The only other feature is specifying a regex for the files to run (default is
`/test-.+\.js$/`), for example:

```js
require('urun')(__dirname, /.+Test\.js$/);
```

## License

This module is licensed under the MIT license.
