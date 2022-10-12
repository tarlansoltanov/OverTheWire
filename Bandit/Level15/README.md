# [Level 15](https://overthewire.org/wargames/bandit/bandit15.html)

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to `port 30000 on localhost`.

## Commands you may need to solve this level

    ssh, telnet, nc, openssl, s_client, nmap

## Authentication Details

    Username : bandit14
    Password : fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit14

nc localhost 30000

fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq
```

## Password for next level

    jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt