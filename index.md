# JS Base SDK For Kuknos Network Developement

This library is the lowest-level kukos helper library. It consists
of classes to read, write, hash, and sign the xdr structures that are used in
kuknos-core This is an
implementation in JavaScript that can be used on either Node.js or web browsers.

- **[API Reference](https://stellar.github.io/js-stellar-base/)**

> **Warning!** Node version of this package is using
> [`sodium-native`](https://www.npmjs.com/package/sodium-native) package, a
> native implementation of [Ed25519](https://ed25519.cr.yp.to/) in Node.js, as
> an
> [optional dependency](https://docs.npmjs.com/files/package.json#optionaldependencies).
> This means that if for any reason installation of this package fails,
> `JS SDK` will fallback to the much slower implementation contained in
> [`tweetnacl`](https://www.npmjs.com/package/tweetnacl).
>
> If you are using `JS SDK` in a browser you can ignore this. However, for
> production backend deployments you should definitely be using `sodium-native`.
> If `sodium-native` is successfully installed and working
> `StellarBase.FastSigning` variable will be equal `true`. Otherwise it will be
> `false`.

## Quick start

Using npm to include kuknos-public-sdk-js in your own project:

```shell
npm install --save kuknos-public-sdk-js
```

## License
kuknos-public-sdk-js is a modified version of [js-stellar-base](https://github.com/stellar/js-stellar-base) which is licensed under an Apache-2.0 license. See the
[LICENSE](./LICENSE) file for details.
