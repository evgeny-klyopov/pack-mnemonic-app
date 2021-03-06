# App pack mnemonic
Console application for pack mnemonic

### [Install](./docs/INSTALL.md)
### How it works?
1. Convert mnemonic to number format by package [wordlist](https://github.com/tyler-smith/go-bip39/tree/master/wordlists)
2. Converting a number (mnemonic) to a format %04d (example 23 -> 0023, 1455 -> 1455, 1 -> 0001)
3. Joining all mnemonic numbers into a string and after remove leading zeros (base10)
5. Convert of the received number into the number system 36 (base36) and 62 (base62)


### Options
* ```--phrase, -p``` - mnemonic phrase
* ```--operation, -o``` - operation (pack/unpack) (default: "pack")
* ```--base, -b``` - base (10/36/62) (default: "10")
* ```--lang, -l ``` - lang (English/Czech/French/Italian/Japanese/Korean/Spanish/ChineseTraditional/ChineseSimplified) (default: "English")

### Run
```shell
pm -p="able 1644 awful crisp collect claim educate can ball toy wealth spell window young reveal zone review kit decorate delay defy air pear brave"
pm -p="39fm2qxfr0t4w4mb3ao815pjlpw79kajluui4f5c578ebyhmkmplvyfmz6ca" -o="unpack" -b=36

```
![Output](./docs/img/output.png "Output")
