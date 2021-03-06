# go-ethereum-vanitygen
Vanitygen for Ethereum. Supports for specific prefix or suffix. 
The purposes are for learning Golang and generating Ethereum address for PoC of short address attack on Ethereum.

## Installation
```
go get github.com/chrsow/geth-vanitygen
```

## Features
`prefix` searchig address for specific prefix. (`-p` option)

`suffix` searchig address for specific suffix. (`-s` option)

(Ethereum address is in `hexadecimal` format.)

## Examples
```
// search for eth. address with prefix beef
# geth-vanitygen -p beef
[+] Address with prefix "beef" found.
Address: 0xbeef.....
PrivateKey: 52.....

// search for eth. address with suffix 00
# geth-vanitygen -s 00
[+] Address with suffix "00" found.
Address: 0x2f.....00
PrivateKey: 81.....

// no option, search for default eth. address
# geth-vanitygen
[+] Generate Ethereum address
Address: 0x25.....
PrivateKey: 5f.....
```
