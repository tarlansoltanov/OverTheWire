# [Level 16](https://overthewire.org/wargames/bandit/bandit16.html)

## Level Goal

The password for the next level can be retrieved by submitting the password of the current level to `port 30001 on localhost` using SSL encryption.

`Helpful note: Getting “HEARTBEATING” and “Read R BLOCK”? Use -ign_eof and read the “CONNECTED COMMANDS” section in the manpage. Next to ‘R’ and ‘Q’, the ‘B’ command also works in this version of that command…`

## Commands you may need to solve this level

    ssh, telnet, nc, openssl, s_client, nmap

## Authentication Details

    Username : bandit15
    Password : jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit15

openssl s_client localhost:30001

jN2kgmIXJ6fShzhT2avhotn4Zcka6tnt
```

## Password for next level

    JQttfApK4SeyHwDlI9SXGR50qclOAil1