# Safer CBOR in Go

Safer CBOR provides secure CBOR encoding and decoding with [fxamacker/cbor](https://github.com/fxamacker/cbor).

Package cbor provides helper functions for encoding and decoding CBOR using the [Go](https://golang.org) programming language.

1. CBOR is encoded using Core Deterministic Encoding defined in RFC 8949, which obsoletes Canonical CBOR defined in RFC 7049.

2. CBOR decoder detects and rejects duplicate map keys, which is an important requirement in security sensitive applications.

## Performance

There's a tradeoff between performance and security. 

Sorting is slower than not sorting.  Detecting duplicate keys is slower than not detecting them. And so on.

Please don't use this to claim other CBOR libraries using less secure options are faster.

## Installation

Copy cbor.go.txt as cbor.go into your project and use.

## CBOR Resources

For more info, see:
  * github.com/fxamacker/cbor
  * github.com/x448/safer-cbor

## License

safer-cbor is licensed under the MIT License.  See [LICENSE] file for the full text of the license.

Copyright © 2021 Montgomery Edwards⁴⁴⁸
