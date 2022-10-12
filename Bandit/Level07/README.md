# [Level 7](https://overthewire.org/wargames/bandit/bandit7.html)

## Level Goal

The password for the next level is stored `somewhere on the server` and has all of the following properties:

* owned by user bandit7
* owned by group bandit6
* 33 bytes in size

## Commands you may need to solve this level

    ls, cd, cat, file, du, find, grep

## Authentication Details

    Username : bandit6
    Password : P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit6

find / -user bandit7 -group bandit6 -size 33c 2>/dev/null

cat /var/lib/dpkg/info/bandit7.password
```

## Password for next level

    z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S