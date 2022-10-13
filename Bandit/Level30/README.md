# [Level 30](https://overthewire.org/wargames/bandit/bandit30.html)

## Level Goal

There is a git repository at ssh://bandit29-git@localhost/home/bandit29-git/repo. The password for the user bandit29-git is the same as for the user bandit29.

Clone the repository and find the password for the next level.

## Commands you may need to solve this level

    git

## Authentication Details

    Username : bandit29
    Password : tQKvmcwNYcFS6vmPHIUSI3ShmsrQZK8S

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit29

mkdir /tmp/myname123/

cd /tmp/myname123/

git clone ssh://bandit29-git@localhost:2220/home/bandit29-git/repo

cd repo/

git branch -a

git switch dev

cat README.md
```

## Password for next level

    xbhV3HpNGlTIdnjUrdAlPzc2L6y9EOnS