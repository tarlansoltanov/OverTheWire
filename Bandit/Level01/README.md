# [Level 1](https://overthewire.org/wargames/bandit/bandit1.html)

## Level Goal

The password for the next level is stored in a file called readme located in the home directory. Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

## Commands you may need to solve this level

    ls, cd, cat, file, du, find

## Authentication Details

    Username : bandit0
    Password : bandit0

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit0

cat readme
```

## Password for next level

    NH2SXQwcBdpmTEzi3bvBHMM9H66vVXjL 