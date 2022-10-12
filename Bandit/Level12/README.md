# [Level 12](https://overthewire.org/wargames/bandit/bandit12.html)

## Level Goal

The password for the next level is stored in the file `data.txt`, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Commands you may need to solve this level

    grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Authentication Details

    Username : bandit11
    Password : 6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit11

cat data.txt | tr -t "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz" "NOPQRSTUVWXYZABCDEFGHIJKLMnopqrstuvwxyzabcdefghijklm"
```

## Password for next level

    JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv