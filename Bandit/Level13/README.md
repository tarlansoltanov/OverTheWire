# [Level 13](https://overthewire.org/wargames/bandit/bandit13.html)

## Level Goal

The password for the next level is stored in the file `data.txt`, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work using mkdir. For example: mkdir /tmp/myname123. Then copy the datafile using cp, and rename it using mv (read the manpages!)

## Commands you may need to solve this level

    grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

## Authentication Details

    Username : bandit12
    Password : JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

## Solution Steps

``` 
ssh bandit.labs.overthewire.org -p 2220 -l bandit12

mkdir /tmp/myname123

cp data.txt /tmp/myname123

cd /tmp/myname123

xxd -r data.txt > data2.txt

file data2.txt

mv data2.txt data3.gz

gzip -d data3.gz

file data3

mv data3 data4.bz2

bzip2 -d data4.bz2

file data4

mv data4 data5.gz

gzip -d data5.gz

file data5

mv data5 data6.tar

tar -xf data6.tar

file data5.bin

mv data5.bin data7.tar

tar -xf data7.tar

file data6.bin

mv data6.bin data8.bz2

bzip2 -d data8.bz2

file data8

mv data8 data9.tar

tar -xf data9.tar

file data8.bin

mv data8.bin data10.gz

gzip -d data10.gz

file data10

cat data10
```

## Password for next level

    wbWdlBxEir4CaE8LaPhauuOo6pwRmrDw