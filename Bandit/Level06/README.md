# [Level 6](https://overthewire.org/wargames/bandit/bandit6.html)

## Level Goal

The password for the next level is stored in a file somewhere under the `inhere` directory and has all of the following properties:

* human-readable
* 1033 bytes in size
* not executable

## Commands you may need to solve this level

    ls, cd, cat, file, du, find

## Authentication Details

    Username : bandit5
    Password : lrIWWI6bB37kxfiCQZqUdOIYfr6eEeqR

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit5

find ./inhere/ -size 1033c ! -executable -exec file {} \; | grep ASCII

cat ./inhere/maybehere07/.file2
```

## Password for next level

    P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU