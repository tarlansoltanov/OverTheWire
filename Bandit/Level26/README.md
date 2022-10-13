# [Level 26](https://overthewire.org/wargames/bandit/bandit26.html)

## Level Goal

Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not `/bin/bash`, but something else. Find out what it is, how it works and how to break out of it.

## Commands you may need to solve this level

    ssh, cat, more, vi, ls, id, pwd

## Authentication Details

    Username : bandit25
    Password : p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit25

stty rows 2

ssh -i bandit26.sshkey bandit26@localhost -p 2220

v

:e /etc/bandit_pass/bandit26
```

## Password for next level

    c7GvcKlw9mC7aUQaPx7nwFstuAIBw1o1