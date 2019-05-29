<img src="http://myntcore.io/css/images/module-mnemonic.png" alt="myntcore mnemonics" height="35">
BIP39 Mnemonics for myntcore
=======

[![NPM Package](https://img.shields.io/npm/v/myntcore-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/myntcore-mnemonic)
[![Build Status](https://img.shields.io/travis/myntdevkit/myntcore-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/myntdevkit/myntcore-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/myntdevkit/myntcore-mnemonic.svg?style=flat-square)](https://coveralls.io/r/myntdevkit/myntcore-mnemonic)

A module for [myntcore](https://github.com/myntdevkit/myntcore) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install myntcore-mnemonic
bower install myntcore-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://myntcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('myntcore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/myntdevkit/myntcore/blob/master/CONTRIBUTING.md) on the main myntcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/myntdevkit/myntcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
