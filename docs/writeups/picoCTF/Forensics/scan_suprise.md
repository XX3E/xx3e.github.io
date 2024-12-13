---
title: Scan Suprise
parent: Forensics
---

In this CTF i was suprised with a file named *flag.png*.
After opening it i found a qr code. Because it is not always possible to open and scan with a camera i searched for a solution to extract the flag from my terminal.

1. install zbar-tools
```
sudo apt install zbar-tools
```
2. extract the content of the file
```
zbarimg -q --raw flag.png
```