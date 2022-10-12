# [Level 4](https://overthewire.org/wargames/bandit/bandit4.html)

## Level Goal

The password for the next level is stored in a hidden file in the `inhere` directory.

## Commands you may need to solve this level

    ls, cd, cat, file, du, find

## Authentication Details

    Username : bandit3
    Password : aBZ0W5EmUfAf7kHTQeOwd8bauFJ2lAiG

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit3

ls -a ./inhere/

cat ./inhere/.hidden
```

## Password for next level

    2EW7BBsr6aMMoJ2HjW067dm8EgX26xNe