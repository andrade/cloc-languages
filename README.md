New language processing filters for [cloc](https://github.com/AlDanial/cloc).

```
$ cloc --read-lang-def=cloc-extra-langs <FILE|DIR> ...
```

### Example

```
$ cloc --ignored=ignored sgx.edl
       1 text file.
       1 unique file.
Wrote ignored
       1 file ignored.

$ more ignored
sgx.edl: language unknown (#3)

$ cloc --ignored=ignored --read-lang-def=cloc-extra-langs sgx.edl
       1 text file.
       1 unique file.
Wrote ignored
       0 files ignored.

github.com/AlDanial/cloc v 1.74  T=0.01 s (169.5 files/s, 35925.5 lines/s)
-------------------------------------------------------------------------------
Language                     files          blank        comment           code
-------------------------------------------------------------------------------
EDL                              1             15            155             42
-------------------------------------------------------------------------------
```
