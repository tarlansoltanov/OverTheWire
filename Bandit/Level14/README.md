# [Level 14](https://overthewire.org/wargames/bandit/bandit14.html)

## Level Goal

The password for the next level is stored in `/etc/bandit_pass/bandit14 and can only be read by user bandit14`. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level. `Note: localhost` is a hostname that refers to the machine you are working on

## Commands you may need to solve this level

    ssh, telnet, nc, openssl, s_client, nmap

## Authentication Details

    Username : bandit13
    Password : wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit13

ssh -i sshkey.private bandit14@localhost

cat /etc/bandit_pass/bandit14
```

## Password for next level

    fGrHPx402xGC7U7rXKDaxiWFTOiF0ENq