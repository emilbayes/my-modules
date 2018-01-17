# My Modules

> A categorised overview of my modules :smile:

## Categories

- [Security & Cryptography]()
- [Buffers]()
-

### Security & Cryptography

#### <code><i>sodium-friends</i>/<b>sodium-native</b></code>

Node.js native bindings to the modern, easy to use cryptography suite [`libsodium`](https://github.com/jedisct1/libsodium). Very low-level, but also
very robust, and brings some unique features to Node.js, such as Secure Buffers,
secret streams, easy encryption, modern hashing etc.

#### <code><i>sodium-friends</i>/<b>sodium-javascript</b></code>

Javascript implementation of a subset of `sodium-native`. Aims to become feature
complete with `libsodium` as far as browsers allow. Also provides WASM
implementations where possible.

#### <code><i>emilbayes</i>/<b>blake2b</b></code>

Implementation of Blake2b hashing function in Javascript with the
personalisation and salt parameters. Upgrades to WASM implementation where
possible for super fast hashing. Forked form [`dcposch/blakejs`](https://github.com/dcposch/blakejs)

#### <code><i>emilbayes</i>/<b>is-secure-buffer</b></code>

Utility to check if a `Buffer` is a `sodium-native` Secure Buffer,
just like `Buffer.isBuffer(buf)`
