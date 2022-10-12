# [Level 8](https://overthewire.org/wargames/bandit/bandit8.html)

## Level Goal

The password for the next level is stored in the file `data.txt` next to the word `millionth`

## Commands you may need to solve this level

    man, grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Authentication Details

    Username : bandit7
    Password : z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit7

cat data.txt | grep millionth
```

## Password for next level

    TESKZC0XvTetK0S9xNwm25STk5iWrBvP