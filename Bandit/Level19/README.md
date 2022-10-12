# [Level 19](https://overthewire.org/wargames/bandit/bandit19.html)

## Level Goal

There are 2 files in the homedirectory: `passwords.old and passwords.new`. The password for the next level is in `passwords.new` and is the only line that has been changed between `passwords.old and passwords.new`

`NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19`

## Commands you may need to solve this level

    ssh, ls, cat

## Authentication Details

    Username : bandit18
    Password : hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit18 "cat readme"
```

## Password for next level

    awhqfNnAbc1naukrpqDYcF95h7HoMTrC