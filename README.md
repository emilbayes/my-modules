# My Modules

> A categorised overview of my modules :smile:

## Categories

- [Security & Cryptography]()
- [Buffers]()
-

### Security & Cryptography

#### [<code><i>sodium-friends</i>/<b>sodium-native</b></code>](https://github.com/sodium-friends/sodium-native]

Node.js native bindings to the modern, easy to use cryptography suite [`libsodium`](https://github.com/jedisct1/libsodium). Very low-level, but also
very robust, and brings some unique features to Node.js, such as Secure Buffers,
secret streams, easy encryption, modern hashing etc.

#### [<code><i>sodium-friends</i>/<b>sodium-javascript</b></code>](https://github.com/sodium-friends/sodium-javascript]

Javascript implementation of a subset of `sodium-native`. Aims to become feature
complete with `libsodium` as far as browsers allow. Also provides WASM
implementations where possible.

#### [<code><i>emilbayes</i>/<b>blake2b</b></code>](https://github.com/emilbayes/blake2b

Implementation of Blake2b hashing function in Javascript with the
personalisation and salt parameters. Upgrades to WASM implementation where
possible for super fast hashing. Forked form [`dcposch/blakejs`](https://github.com/dcposch/blakejs)

#### [<code><i>emilbayes</i>/<b>secure-random-uniform</b></code>](https://github.com/emilbayes/secure-random-uniform]

Generate random integers uniformly in a range. A secure drop in for where you'd
normally use `Math.random` in user facing scenarios (which is almost always).
Can generate integers in `[0, 2^53 - 1)` (which is `Number.MAX_SAFE_INTEGER`).
Uses `libsodium`s CSPRNG (Cryptographically Secure Pseudo Random Number Generator)

#### [<code><i>emilbayes</i>/<b>secure-random-shuffle</b></code>](https://github.com/emilbayes/secure-random-shuffle]

Shuffle an array using a secure random number generator, which is almost always
what you want in a user facing scenario. Based on `emilbayes/secure-random-uniform`

#### [<code><i>emilbayes</i>/<b>secure-random-sample</b></code>](https://github.com/emilbayes/secure-random-shuffle]

Randomly pick `n` out of `k` integers without replacement, using a secure random
number generator. The integers could be indexes into an array or ids. Based on
`emilbayes/secure-random-uniform`.

#### [<code><i>emilbayes</i>/<b>is-secure-buffer</b></code>](https://github.com/emilbayes/is-secure-buffer]

Utility to check if a `Buffer` is a `sodium-native` Secure Buffer,
just like `Buffer.isBuffer(buf)`
