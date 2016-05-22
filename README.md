# Hello world Linux module

## Install linux headers
apt-get install build-essential linux-headers-$(uname -r)

## Make
make

## Install 
insmod hello.ko

dmesg | tail -1

Hello world!

## Uninstall
rmmod hello.ko

dmesg | tail -1

Cleaning up module
