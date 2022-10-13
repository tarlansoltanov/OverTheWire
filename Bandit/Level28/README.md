# [Level 28](https://overthewire.org/wargames/bandit/bandit28.html)

## Level Goal

There is a git repository at ssh://bandit27-git@localhost/home/bandit27-git/repo. The password for the user bandit27-git is the same as for the user bandit27.

Clone the repository and find the password for the next level.

## Commands you may need to solve this level

    git

## Authentication Details

    Username : bandit27
    Password : YnQpBuifNMas1hcUFk70ZmqkhUU2EuaS

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit27

mkdir /tmp/myname123/

cd /tmp/myname123/

git clone ssh://bandit27-git@localhost:2220/home/bandit27-git/repo

cat repo/README
```

## Password for next level

    AVanL161y9rsbcJIsFHuw35rjaOM19nR