---
title: Verify
parent: Forensics
---

{: .note-title }
> CTF
>
> *People keep trying to trick my players with imitation flags. I want to make sure they get the real thing! I'm going to provide the SHA-256 hash and a decrypt script to help you know that my flags are legitimate.*

----

After login with ssh to the instance i found a bash-script in my home dir. There was also  a folder named *files* with many files inside and a file which holds a checksum.

The exercise was to find the right file under *files* with the checksum from *checksum.txt* and decrypt it with the *decrypt.sh*

1. get checksum from files with [[sha256sum]] and [[grep]] line which fits to logged checksum
```
sha256sum ./files/* | grep $(cat ../checksum.txt)
```
2. decrypt matching file 
```
./decrypt.sh ./files/87590c24
```

