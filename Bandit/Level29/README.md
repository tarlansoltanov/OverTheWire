# [Level 29](https://overthewire.org/wargames/bandit/bandit29.html)

## Level Goal

There is a git repository at ssh://bandit28-git@localhost/home/bandit28-git/repo. The password for the user bandit28-git is the same as for the user bandit28.

Clone the repository and find the password for the next level.

## Commands you may need to solve this level

    git

## Authentication Details

    Username : bandit28
    Password : AVanL161y9rsbcJIsFHuw35rjaOM19nR

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit28

mkdir /tmp/myname123/

cd /tmp/myname123/

git clone ssh://bandit28-git@localhost:2220/home/bandit28-git/repo

cd repo/

git log --oneline

git show bdf3099
```

## Password for next level

    tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S