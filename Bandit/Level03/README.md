# [Level 3](https://overthewire.org/wargames/bandit/bandit3.html)

## Level Goal

The password for the next level is stored in a file called `spaces in this filename` located in the home directory

## Commands you may need to solve this level

    ls, cd, cat, file, du, find

## Authentication Details

    Username : bandit2
    Password : rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit2

cat "spaces in this filename"
```

## Password for next level

    aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG