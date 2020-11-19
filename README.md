<p align="center">
  <img src="assets/logo/web3js.jpg" width="200" alt="web3.js" />
</p>

# gncweb3.js - GNC JavaScript API

[![Gitter][gitter-image]][gitter-url] [![StackExchange][stackexchange-image]][stackexchange-url] [![NPM Package Version][npm-image-version]][npm-url] [![NPM Package Downloads][npm-image-downloads]][npm-url] [![Build Status][actions-image]][actions-url] [![Dev Dependency Status][deps-dev-image]][deps-dev-url] [![Coverage Status][coveralls-image]][coveralls-url] [![Lerna][lerna-image]][lerna-url] [![Netlify Status][netlify-image]][netlify-url]

This is the GNC [JavaScript API][docs]

## Installation

### Node

```bash
npm install gncweb3
```


### In the Browser

Use the prebuilt `dist/gncweb3.min.js`, or
build using the [gncweb3.js][repo] repository:

```bash
npm run build
```

Then include `dist/gncweb3.min.js` in your html file.
This will expose `Web3` on the window object.


## Usage

```js
// In Node.js
const Web3 = require('gncweb3');

let web3 = new Web3('ws://localhost:8546');
console.log(web3);
> {
    eth: ... ,
    shh: ... ,
    utils: ...,
    ...
}
```

Additionally you can set a provider using `web3.setProvider()` (e.g. WebsocketProvider):

```js
web3.setProvider('ws://localhost:8546');
// or
web3.setProvider(new Web3.providers.WebsocketProvider('ws://localhost:8546'));
```

There you go, now you can use it:

```js
web3.eth.getAccounts().then(console.log);
```

### Usage with TypeScript

We support types within the repo itself. Please open an issue here if you find any wrong types.

You can use `web3.js` as follows:

```typescript
import Web3 from 'gncweb3';
const web3 = new Web3('ws://localhost:8546');
```

If you are using the types in a `commonjs` module, like in a Node app, you just have to enable `esModuleInterop` and `allowSyntheticDefaultImports` in your `tsconfig` for typesystem compatibility:

```js
"compilerOptions": {
    "allowSyntheticDefaultImports": true,
    "esModuleInterop": true,
    ....
```

## Documentation

Documentation can be found at [ReadTheDocs][docs].

## Building

### Requirements

-   [Node.js](https://nodejs.org)
-   [npm](https://www.npmjs.com/)

```bash
sudo apt-get update
sudo apt-get install nodejs
sudo apt-get install npm
```

### Building (webpack)

Build the web3.js package:

```bash
npm run build
```

### Testing (mocha)

```bash
npm test
```

