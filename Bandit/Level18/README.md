# [Level 18](https://overthewire.org/wargames/bandit/bandit18.html)

## Level Goal

There are 2 files in the homedirectory: `passwords.old and passwords.new`. The password for the next level is in `passwords.new` and is the only line that has been changed between `passwords.old and passwords.new`

`NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19`

## Commands you may need to solve this level

    cat, grep, ls, diff

## Authentication Details

    Username : bandit17
    Password : VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit17

diff passwords.new passwords.old | grep "<" | cut -d " " -f 2
```

## Password for next level

    hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg