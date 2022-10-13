# [Level 23](https://overthewire.org/wargames/bandit/bandit23.html)

## Level Goal

A program is running automatically at regular intervals from `cron`, the time-based job scheduler. Look in `/etc/cron.d/` for the configuration and see what command is being executed.

`NOTE:` Looking at shell scripts written by other people is a very useful skill. The script for this level is intentionally made easy to read. If you are having problems understanding what it does, try executing it to see the debug information it prints.

## Commands you may need to solve this level

    cron, crontab, crontab(5) (use “man 5 crontab” to access this)

## Authentication Details

    Username : bandit22
    Password : WdDozAdTM2z9DiFEQ2mGlwngMfj4EZff

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit22

ls /etc/cron.d

cat /etc/cron.d/cronjob_bandit23

cat /usr/bin/cronjob_bandit23.sh

echo I am user bandit23 | md5sum | cut -d ' ' -f 1

cat /tmp/8169b67bd894ddbb4412f91573b38db3
```

## Password for next level

    QYw0Y2aiA672PsMmh9puTQuhoz8SyR2G