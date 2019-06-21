# Raspberry
## Requirements
### Electronics
Raspberry Pi
SD Card 4 Gb minimum
USB 4 Gb minimum
### OS Image
DietPi - 21/06/2019
## Steps
### Step 1
Install the operative system in the sd card. (Etcher)
### Step Optional
Config raspberry pi to enable some settings
### Step 2
Connect to raspberry pi with ssh


### Annex 2 - How to make a USB stick swap disk?

https://askubuntu.com/questions/173676/how-to-make-a-usb-stick-swap-disk

1) Make sure your USB stick is connected. In a terminal type:

sudo blkid

It will list all your connected drives. Search for your USB stick you want to use as swap and copy the UUID (everything inside these quotes UUID="XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX").

This represents the individual name of your device.

Also note the /dev/XXX point of your device.

2) Now unmount your device by typing:

sudo umount /dev/XXX (where XXX represents your device name)

3) Format your USB stick as swap, e.g. by terminal

sudo mkswap /dev/XXX (<-- be sure to use the correct device name here or you'll probably end up formatting the wrong drive!)

or simply use GParted.

4) Now you have to edit your /etc/fstab file, so type

sudo nano /etc/fstab

and enter the following

UUID=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX none swap sw,pri=5 0 0

(for all the Xs, use the UUID number you got by typing sudo blkid)

5) Now type

sudo swapon -a

That's it, this should already work.


## URL
https://dietpi.com/
https://dietpi.com/phpbb/viewtopic.php?f=8&t=9#p9
https://www.raspberrypi.org/documentation/configuration/security.md

