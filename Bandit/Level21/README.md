# [Level 21](https://overthewire.org/wargames/bandit/bandit21.html)

## Level Goal

There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

`NOTE:` Try connecting to your own network daemon to see if it works as you think

## Commands you may need to solve this level

    ssh, nc, cat, bash, screen, tmux, Unix ‘job control’ (bg, fg, jobs, &, CTRL-Z, …)

## Authentication Details

    Username : bandit20
    Password : VxCazJaVykI6W36BkBU0mJTCM8rR95XT

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit20

echo VxCazJaVykI6W36BkBU0mJTCM8rR95XT | nc -l localhost 31111 &

./suconnect 31111
```

## Password for next level

    NvEJF7oVjkddltPSrdKEFOllh9V1IBcq