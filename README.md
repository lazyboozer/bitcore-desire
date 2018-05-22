# Bitcore-Dash

[![NPM Package](https://img.shields.io/npm/v/bitcore-desire.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-desire)
[![Build Status](https://img.shields.io/travis/lazyboozer/bitcore-desire.svg?branch=master&style=flat-square)](https://travis-ci.org/lazyboozer/bitcore-desire)

Infrastructure to build Dash and blockchain-based applications for the next generation of financial technology.

**Note:** If you're looking for the Bitcore-Dash Library please see: https://github.com/lazyboozer/bitcore-lib-desire

## Getting Started

Before you begin you'll need to have Node.js v4+ installed. There are several options for installation. One method is to use [nvm](https://github.com/creationix/nvm) to easily switch between different versions, or download directly from [Node.js](https://nodejs.org/).

```bash
npm install -g bitcore-desire
```

Spin up a full node and join the network:

```bash
npm install -g bitcore-desire
bitcored
```

You can then view the Insight block explorer at the default location: `http://localhost:3001/insight`, and your configuration file will be found in your home directory at `~/.bitcore`.

Create a transaction:
```js
var bitcore = require('bitcore-desire');
var transaction = new bitcore.Transaction();
var transaction.from(unspent).to(address, amount);
transaction.sign(privateKey);
```

## Applications

- [Node-Dash](https://github.com/lazyboozer/bitcore-node-desire) - A full node with extended capabilities using Dash Core
- [Insight API-Dash](https://github.com/lazyboozer/insight-api-desire) - A blockchain explorer HTTP API
- [Insight UI-Dash](https://github.com/lazyboozer/insight-ui-desire) - A blockchain explorer web user interface
- [Wallet Service](https://github.com/lazyboozer/bitcore-wallet-service-desire) - A multisig HD service for wallets
- [Wallet Client](https://github.com/lazyboozer/bitcore-wallet-client-desire) - A client for the wallet service
- CLI Wallet - A command-line based wallet client
- Angular Wallet Client - An Angular based wallet client
- Copay - An easy-to-use, multiplatform, multisignature, secure Dash wallet

## Libraries

- [Lib-Dash](https://github.com/lazyboozer/bitcore-lib-desire) - All of the core Dash primatives including transactions, private key management and others
- Payment Protocol - A protocol for communication between a merchant and customer
- [P2P-Dash](https://github.com/lazyboozer/bitcore-p2p-desire) - The peer-to-peer networking protocol
- [Mnemonic-Dash](https://github.com/lazyboozer/bitcore-mnemonic-desire) - Implements mnemonic code for generating deterministic keys
- Channel - Micropayment channels for rapidly adjusting Dash transactions
- [Message-Dash](https://github.com/lazyboozer/bitcore-message-desire) - Dash message verification and signing
- [ECIES-Dash](https://github.com/lazyboozer/bitcore-ecies-desire) - Uses ECIES symmetric key negotiation from public keys to encrypt arbitrarily long data streams.

## Documentation

The complete docs are hosted here: [bitcore documentation](http://bitcore.io/guide/). There's also a [bitcore API reference](http://bitcore.io/api/) available generated from the JSDocs of the project, where you'll find low-level details on each bitcore utility.

- [Read the Developer Guide](http://bitcore.io/guide/)
- [Read the API Reference](http://bitcore.io/api/)

To get community assistance and ask for help with implementation questions, please use our [community forums](http://bitpaylabs.com/c/bitcore).

## Security

We're using Bitcore in production, as are [many others](http://bitcore.io#projects), but please use common sense when doing anything related to finances! We take no responsibility for your implementation decisions.

If you find a security issue, please email security@bitpay.com.

## Contributing

Please send pull requests for bug fixes, code optimization, and ideas for improvement. For more information on how to contribute, please refer to our [CONTRIBUTING](https://github.com/lazyboozer/bitcore-desire/blob/master/CONTRIBUTING.md) file.

This will generate files named `bitcore.js` and `bitcore.min.js`.

## License

Released under the MIT license, under the same terms as DashCore itself. See [LICENSE](LICENSE) for more info.
