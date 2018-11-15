# Linux SysAdmin Journal
I am doing this journal to keep track of useful commands, macros, softwares, configurations to manage a linux system.


## Subdirecttories:
```
|___ https://github.com/H3xFiles/linuxKernelDev_journal <--- Developing
|___ https://github.com/H3xFiles/SOC_journal  <--- Hardening, Incident response, network-hunting
```


- https://www.cyberciti.biz 
- [understanding-log-files-in-linux-where-to-look-when-things-go-wrong](http://www.lostsaloon.com/technology/understanding-log-files-in-linux-where-to-look-when-things-go-wrong/)


### 15/11/2018
Copy file from HD to USB stick from cmd line.

#### find the USB key: check the sdbx where x is a number
```Bash
lsblk

sdb
|___sdb1
```
#### Make a mount point
```Bash
mkdir /mnt/usbstick
```
#### Mount the partition
```Bash
mount /dev/sdb1 /mnt/usbstick
```
#### Copy files
```Bash
cp -r /myApp/ /dev/sdb1/
```
#### Unmount
```Bash
umount /mnt/usbstick
```
