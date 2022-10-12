# [Level 10](https://overthewire.org/wargames/bandit/bandit10.html)

## Level Goal

The password for the next level is stored in the file `data.txt` in one of the few human-readable strings, preceded by several ‘=’ characters.

## Commands you may need to solve this level

    grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Authentication Details

    Username : bandit9
    Password : EN632PlfYiZbn3PhVK3XOGSlNInNE00t

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit9

strings -e s data.txt | grep "^=="
```

## Password for next level

    G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s