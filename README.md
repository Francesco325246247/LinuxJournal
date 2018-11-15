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

#### Copy file from HD to USB stick from cmd line.

```Bash
lsblk
sdb
|___sdb1   <---- USB key

#### Make a mount point
mkdir /mnt/usbstick

#### Mount the partition
mount /dev/sdb1 /mnt/usbstick

#### Copy files
cp -r /myApp/ /dev/sdb1/

#### Unmount
umount /mnt/usbstick
```

Links:
- [Error on Ubuntu boot up - “recovering journal” ](https://askubuntu.com/questions/924170/error-on-ubuntu-boot-up-recovering-journal)
- [Copying files to a USB drive](https://askubuntu.com/questions/37767/how-to-access-a-usb-flash-drive-from-the-terminal)
- [How to access a usb flash drive from the terminal?](https://askubuntu.com/questions/37767/how-to-access-a-usb-flash-drive-from-the-terminal)
- [How to show only hidden files in Terminal?](https://askubuntu.com/questions/468901/how-to-show-only-hidden-files-in-terminal)
- [How To Read and Set Environmental and Shell Variables on a Linux](https://www.digitalocean.com/community/tutorials/how-to-read-and-set-environmental-and-shell-variables-on-a-linux-vps)
