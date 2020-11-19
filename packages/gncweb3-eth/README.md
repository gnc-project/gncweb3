# gncweb3-eth

[![NPM Package][npm-image]][npm-url] [![Dependency Status][deps-image]][deps-url] [![Dev Dependency Status][deps-dev-image]][deps-dev-url]

This is a sub-package of [web3.js][repo].

This Eth package is used within some [web3.js][repo] packages.

Please read the [documentation][docs] for more.

## Installation

### Node.js

```bash
npm install gncweb3-eth
```

## Usage

```js
const Web3Eth = require('gncweb3-eth');

const eth = new Web3Eth('ws://localhost:8546');
```

## Types

All the TypeScript typings are placed in the `types` folder.

[docs]: http://web3js.readthedocs.io/en/1.0/
[repo]: https://github.com/ethereum/gncweb3-eth.js
[npm-image]: https://img.shields.io/npm/v/gncweb3-eth.svg
[npm-url]: https://npmjs.org/package/gncweb3-eth
[deps-image]: https://david-dm.org/ethereum/web3.js/1.x/status.svg?path=packages/gncweb3-eth
[deps-url]: https://david-dm.org/ethereum/web3.js/1.x?path=packages/gncweb3-eth
[deps-dev-image]: https://david-dm.org/ethereum/web3.js/1.x/dev-status.svg?path=packages/gncweb3-eth
[deps-dev-url]: https://david-dm.org/ethereum/web3.js/1.x?type=dev&path=packages/gncweb3-eth
