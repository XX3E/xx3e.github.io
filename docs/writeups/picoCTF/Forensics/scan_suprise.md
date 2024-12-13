---
title: Scan Suprise
parent: Forensics
---

# Scan Suprise

{: .CTF_INSTRUCTIONS }
> CTF Instructions
>
> Author: Jeffery John
> 
> I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead? You can download the challenge files here:
>
>  challenge.zip


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
