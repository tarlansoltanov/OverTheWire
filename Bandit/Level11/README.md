# [Level 11](https://overthewire.org/wargames/bandit/bandit11.html)

## Level Goal

The password for the next level is stored in the file `data.txt`, which contains base64 encoded data

## Commands you may need to solve this level

    grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Authentication Details

    Username : bandit10
    Password : G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit10

base64 -d data.txt
```

## Password for next level

    6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM