BLAKE
=====

Reference implementation of the SHA-3 finalist BLAKE, a family of
cryptographic hash functions composed of 4 instances:
* BLAKE-224
* BLAKE-256
* BLAKE-384
* BLAKE-512

These implementations aim to simplicity and compactness rather than
performance.

BLAKE was designed by [Jean-Philippe Aumasson](https://131002.net) with
Luca Henzen, Willi Meier, and Raphael C.-W. Phan.

[BLAKE2](https://blake2.net) is an improved version of BLAKE, which has
its [own code repo](https://github.com/BLAKE2/BLAKE2).


Usage
-----

Running

```sh
  make
```

will build the 4 executables `blake224`, `blake256`, `blake384`,
`blake512`. 

```C
  ./blake256
```

verifies 2 test vectors and shows an error message upon failed test,
and

```c
  ./blake256 [file1] [file2] [...]
```

hashes the files passed as arguments.

Similar executables are provided for BLAKE-224, BLAKE-384, and
BLAKE-512.


License
-------

The BLAKE reference code is released under [CC0
license](https://creativecommons.org/publicdomain/zero/1.0/), a public
domain-like licence.


References
----------

The [BLAKE page](https://131002.net/blake) includes
* specifications of BLAKE
* slides of BLAKE presentations at conferences and workshops
* a list of third-party implementations and modules
* references to cryptanalysis results
