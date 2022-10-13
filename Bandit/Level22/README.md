# [Level 22](https://overthewire.org/wargames/bandit/bandit22.html)

## Level Goal

A program is running automatically at regular intervals from `cron`, the time-based job scheduler. Look in `/etc/cron.d/` for the configuration and see what command is being executed.

## Commands you may need to solve this level

    cron, crontab, crontab(5) (use “man 5 crontab” to access this)

## Authentication Details

    Username : bandit21
    Password : NvEJF7oVjkddltPSrdKEFOllh9V1IBcq

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit21

ls /etc/cron.d

cat /etc/cron.d/cronjob_bandit22

cat /usr/bin/cronjob_bandit22.sh

cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
```

## Password for next level

    WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff