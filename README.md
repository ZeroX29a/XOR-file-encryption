# XOR File Encryption #


> JCtine
This work is a dreivattion of the [project done by simon](https://github.com/mightbesimon/XOR-file-encryption)

Encrypts files with a password byte-by-byte using a XOR cipher.
##New!
* Added Reversing the File as a block: File is broken into blocks of size given by the user and the block is reversed and replaced.
* This Prevents decryption by bruteforcing the Password 

Decryption is the same process,  
only the password *used to encrypt* will decrypt the file.

### compile ###

```bash
$ gcc enc.c -o xore
$ gcc dec.c -o xord
$ gcc both.c -o xorb
```

### usage ###

```
$ ./xorb <mode[-e or -d]> <filename> <password> <reversing block size[<16]>
```

### example ###
```bash
$ ./xorb -e auckland.jpg password1 13
```
will produce `rauckland.jpg` file, to decrypt:
```bash
$ ./xorb -d rauckland.jpg password1 13
```
`rrauckland.jpg` will be identical to the original

## Authors ##
- **JCtine** - [ZeroX29a](https://github.com/ZeroX29a)
- **simon** - [mightbesimon](https://github.com/mightbesimon)

## License ##

MIT

## Acknowledgments ##

- **these are just my sample codes, if you misuse them its not my problem**
