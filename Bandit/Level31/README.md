# [Level 31](https://overthewire.org/wargames/bandit/bandit31.html)

## Level Goal

There is a git repository at ssh://bandit30-git@localhost/home/bandit30-git/repo. The password for the user bandit30-git is the same as for the user bandit30.

Clone the repository and find the password for the next level.

## Commands you may need to solve this level

    git

## Authentication Details

    Username : bandit30
    Password : xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit30

mkdir /tmp/myname123/

cd /tmp/myname123/

git clone ssh://bandit30-git@localhost:2220/home/bandit30-git/repo

cd repo/

git tag

git show secret
```

## Password for next level

    OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt