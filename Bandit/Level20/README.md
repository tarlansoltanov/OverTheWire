# [Level 20](https://overthewire.org/wargames/bandit/bandit20.html)

## Level Goal

To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

## Authentication Details

    Username : bandit19
    Password : awhqfNnAbc1naukrpqDYcF95h7HoMTrC

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit19

./bandit20-do cat /etc/bandit_pass/bandit20
```

## Password for next level

    VxCazJaVykI6W36BkBU0mJTCM8rR95XT