# [Level 5](https://overthewire.org/wargames/bandit/bandit5.html)

## Level Goal

The password for the next level is stored in the only human-readable file in the `inhere` directory. Tip: if your terminal is messed up, try the “reset” command.

## Commands you may need to solve this level

    ls, cd, cat, file, du, find

## Authentication Details

    Username : bandit4
    Password : 2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit4

file ./inhere/* | grep ASCII

cat ./inhere/-file07
```

## Password for next level

    lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR