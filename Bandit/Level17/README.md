# [Level 17](https://overthewire.org/wargames/bandit/bandit17.html)

## Level Goal

The credentials for the next level can be retrieved by submitting the password of the current level to `a port on localhost in the range 31000 to 32000`. First find out which of these ports have a server listening on them. Then find out which of those speak SSL and which don’t. There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

## Commands you may need to solve this level

    ssh, telnet, nc, openssl, s_client, nmap

## Authentication Details

    Username : bandit16
    Password : JQttfApK4SeyHwDlI9SXGR50qclOAil1

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit16

nmap -sV -p31000-32000 localhost

echo JQttfApK4SeyHwDlI9SXGR50qclOAil1 | openssl s_client -quiet localhost:31790 | tail -n +2 > /tmp/myname123/sshkey.private

chmod 600 /tmp/myname123/sshkey.private

ssh -i /tmp/myname123/sshkey.private bandit17@localhost -p 2220

cat /etc/bandit_pass/bandit17
```

## Password for next level

    VwOSWtCA7lRKkTfbr2IDh6awj9RNZM5e