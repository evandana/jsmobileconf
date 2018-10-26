# JavaScript Binary Data

[follow along presentation](kirjs.com/binary/0)

Kir, Firebase

## Take aways

- Use [protobuffers](https://developers.google.com/protocol-buffers/) for serializing structured data
    - Protocol buffers are a language-neutral, platform-neutral extensible mechanism for serializing structured data.


## Binaries

e.g. GIFs

1. Look at simple gif code: `GIF89añ...`
1. Read as binary, adding spacing

## GIFs Binary Explained

1. Header
1. Palette
1. Extensions
1. Semicolon character

## Converting: Binary | Decimal | Hex

- Binary to Decimal: `parseInt('1010101',2)` => `85`
- Decimal to Binary: `(1212).toString(2)` => `10010111100`
- Binary to Hex: `parseInt('01010101', 2).toString(16)` => `55`
- Hex to Binary: `parseInt('FEFEFE', 16).toString(2)` => `111111101111111011111110`

## Unicode

- Char to Unicode: `'lol'.charCodeAt(0)` => `108`
- Unicode to Char: `String.fromCharCode(108)` => `l`

## More References

- [ ] Check out GIF binary generator
- [ ] Graphic Interchage Format standard
- [ ] [GIF Reference](http://giflib.sourceforge.net/whatsinagif/bits_and_bytes.html)
- [ ] [GIF Editors](https://github.com/davisonio/awesome-gif/blob/master/README.md)
- [ ] [Online Hex Editor](https://www.onlinehexeditor.com/)

## [Binary Parser](https://www.npmjs.com/package/binary-parser)

## Binary instead of JSON

### Existing solutions

- Google ProtoBuffers
- Flatbuffers
- Thrift (Apache/Facebook)

## Bonus

- Java class files (in binary) start with `CAFEBABE`