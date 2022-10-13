# [Level 32](https://overthewire.org/wargames/bandit/bandit32.html)

## Level Goal

There is a git repository at ssh://bandit31-git@localhost/home/bandit31-git/repo. The password for the user bandit31-git is the same as for the user bandit31.

Clone the repository and find the password for the next level.

## Commands you may need to solve this level

    git

## Authentication Details

    Username : bandit31
    Password : OoffzGDlzhAlerFJ2cAiz1D41JW1Mhmt

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit31

mkdir /tmp/myname123/

cd /tmp/myname123/

git clone ssh://bandit31-git@localhost:2220/home/bandit31-git/repo

cd repo/

ls -a

rm .gitignore

echo 'May I come in?' > key.txt

git add .

git commit -m "Added key.txt"

git push
```

## Password for next level

    rmCBvG56y58BXzv98yZGdO7ATVL5dW8y