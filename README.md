# NPCcoincore Library

[![Build Status](https://img.shields.io/travis/npccoin/npccoincore-lib.svg?branch=master)](https://travis-ci.org/npccoin/npccoincore-lib)
[![NPM Package](https://img.shields.io/npm/v/npccoincore-lib.svg)](https://www.npmjs.org/package/npccoincore-lib)

> A pure and powerful JavaScript NPCcoin library.

NPCcoin is a powerful new peer-to-peer platform for the next generation of financial technology. The decentralized nature of the NPCcoin network allows for highly resilient NPCcoin infrastructure, and the developer community needs reliable, open-source tools to implement NPCcoin apps and services.

## Table of Contents
- [Install](#install)
- [Usage](#usage)
- [Documentation](#documentation)
- [Contributing](#contributing)
- [License](#license)

## Install

### NodeJS

```
npm install npccoincore-lib
```

### Browser

See the section below to generate your own bundle, or download the pre-generated [minified file](dist/npccoincore-lib.min.js)

#### Building the Browser Bundle

To build a npccoincore-lib full bundle for the browser:

```sh
npm run build
```

This will generate files named `npccoincore-lib.js` and `npccoincore-lib.min.js` in the `dist/` folder.

## Usage

### Browser

```
<script src='./dist/npccoincore-lib.min.js' type="text/javascript"></script>
<script>
  const PrivateKey = npccoincore.PrivateKey;
  const privateKey = new PrivateKey();
  const address = privateKey.toAddress().toString();
</script>
```

### Modules

Some functionality is implemented as a module that can be installed separately:

* [Payment Protocol Support](https://github.com/npccoin/npccoincore-payment-protocol)
* [Peer to Peer Networking](https://github.com/npccoin/npccoincore-p2p)
* [NPCcoin Core JSON-RPC](https://github.com/npccoin/npccoind-rpc)
* [Payment Channels](https://github.com/npccoin/npccoincore-channel)
* [Mnemonics](https://github.com/npccoin/npccoincore-mnemonic)
* [Elliptical Curve Integrated Encryption Scheme](https://github.com/npccoin/bitcore-ecies-npccoin)
* [Signed Messages](https://github.com/npccoin/bitcore-message-npccoin)

### Development & Tests

```sh
git clone https://github.com/npccoin/npccoincore-lib
cd npccoincore-lib
npm install
```

Run all the tests:

```sh
npm test
```

You can also run just the Node.js tests with `npm run test:node`, just the browser tests with `npm run test:browser` or run a test coverage report with `npm run coverage`.

## Documentation

* [Addresses](docs/address.md)
* [Block](docs/block.md)
* [Crypto](docs/crypto.md)
* [Encoding](docs/encoding.md)
* [Hierarchically-derived Private and Public Keys](docs/hierarchical.md)
* [Mnemonic](docs/mnemonic.md)
* [Networks](docs/networks.md)
* [PrivateKey](docs/privatekey.md)
* [PublicKey](docs/publickey.md)
* [Script](docs/script.md)
* [Transaction](docs/transaction.md)
* [Using Different Units](docs/unit.md)
* [Unspent Output](docs/unspentoutput.md)
* [URI](docs/uri.md)
* [Governance Object / Proposal](docs/govobject/govobject.md)

### Examples

Some examples can be found [here](docs/examples.md), below is a list of direct links for some of them.

* [Generate a random address](docs/examples.md#generate-a-random-address)
* [Generate an address from a SHA256 hash](docs/examples.md#generate-a-address-from-a-sha256-hash)
* [Import an address via WIF](docs/examples.md#import-an-address-via-wif)
* [Create a Transaction](docs/examples.md#create-a-transaction)
* [Sign a NPCcoin message](docs/examples.md#sign-a-bitcoin-message)
* [Verify a NPCcoin message](docs/examples.md#verify-a-bitcoin-message)
* [Create an OP RETURN transaction](docs/examples.md#create-an-op-return-transaction)
* [Create a 2-of-3 multisig P2SH address](docs/examples.md#create-a-2-of-3-multisig-p2sh-address)
* [Spend from a 2-of-2 multisig P2SH address](docs/examples.md#spend-from-a-2-of-2-multisig-p2sh-address)

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/npccoin/npccoincore-lib/blob/master/CONTRIBUTING.md) file.

## License

Code released under [the MIT license](LICENSE).

Copyright 2013-2017 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.  
Copyright 2016-2017 The NPCcoin Foundation, Inc.  
Copyright 2017-2018 NPCcoin Core Group, Inc.  
