# [Level 27](https://overthewire.org/wargames/bandit/bandit27.html)

## Level Goal

Good job getting a shell! Now hurry and grab the password for bandit27!

## Commands you may need to solve this level

    ls

## Authentication Details

    Username : bandit26
    Password : c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1

## Solution Steps

``` 
stty rows 6

ssh bandit.labs.overthewire.org -p 2220 -l bandit26

v

:term!/bin/bash

./bandit27-do cat /etc/bandit_pass/bandit27
```

## Password for next level

    YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS