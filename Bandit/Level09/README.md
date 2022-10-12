# [Level 9](https://overthewire.org/wargames/bandit/bandit9.html)

## Level Goal

The password for the next level is stored in the file `data.txt` and is the only line of text that occurs only once

## Commands you may need to solve this level

    grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

## Authentication Details

    Username : bandit8
    Password : TESKZC0XvTetK0S9xNwm25STk5iWrBvP

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit8

cat data.txt | sort | uniq -u
```

## Password for next level

    EN632PlfYiZbn3PhVK3XOGSlNInNE00t