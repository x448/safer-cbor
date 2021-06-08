# Safer CBOR in Go

Safer [CBOR](https://cbor.io) provides secure CBOR encoding and decoding using [fxamacker/cbor](https://github.com/fxamacker/cbor).

It provides helper functions for encoding and decoding CBOR using the [Go](https://golang.org) programming language.

1. CBOR is encoded using Core Deterministic Encoding defined in [RFC 8949](https://tools.ietf.org/html/rfc8949), which obsoletes Canonical CBOR defined in [RFC 7049](https://tools.ietf.org/html/rfc7049).

2. CBOR decoder detects and rejects duplicate map keys, which is an important requirement in security sensitive applications.

## CBOR Installation

Copy cbor.go.txt as cbor.go into your project and use.

## CBOR Resources

For more info, see:
  * https://github.com/fxamacker/cbor
  * https://cbor.io

## CBOR Performance

There's a tradeoff between performance and security. 

Sorting is slower than not sorting.  Detecting duplicate keys is slower than not detecting them. And so on.

Please don't use this to claim other CBOR libraries using less secure options are faster.  Use the same options when comparing.

## License

safer-cbor is licensed under the MIT License.  See [LICENSE] file for the full text of the license.

Copyright © 2021 Montgomery Edwards⁴⁴⁸
