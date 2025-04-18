btcec
=====

[![ISC License](http://img.shields.io/badge/license-ISC-blue.svg)](http://copyfree.org)
[![GoDoc](https://pkg.go.dev/github.com/bcutil/eclib?status.png)](https://pkg.go.dev/github.com/bcutil/eclib)

package eclib implements elliptic curve cryptography needed for working with
Bitcoin (secp256k1 only for now). It is designed so that it may be used with the
standard crypto/ecdsa packages provided with go.  A comprehensive suite of test
is provided to ensure proper functionality.  package eclib was originally based
on work from ThePiachu which is licensed under the same terms as Go, but it has
significantly diverged since then.  The btcsuite developers original is licensed
under the liberal ISC license.

Although this package was primarily written for btcd, it has intentionally been
designed so it can be used as a standalone package for any projects needing to
use secp256k1 elliptic curve cryptography.

## Installation and Updating

```bash
$ go install -u -v github.com/bcutil/eclib
```

## Examples

* [Sign Message](https://pkg.go.dev/github.com/bcutil/eclib#example-package--SignMessage)  
  Demonstrates signing a message with a secp256k1 private key that is first
  parsed form raw bytes and serializing the generated signature.

* [Verify Signature](https://pkg.go.dev/github.com/bcutil/eclib#example-package--VerifySignature)  
  Demonstrates verifying a secp256k1 signature against a public key that is
  first parsed from raw bytes.  The signature is also parsed from raw bytes.

## License

package eclib is licensed under the [copyfree](http://copyfree.org) ISC License
except for btcec.go and btcec_test.go which is under the same license as Go.

