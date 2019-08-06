# Raspberry
## Requirements
### Electronics
- Raspberry Pi 3 Model B
- SD Card 4 Gb minimum, for install OS (SDCARD1) 
- HDD USB 2.0
- (Optional) USB 4 Gb minimum
- (Optional - Recycle or old) SD 1 or 2 GB for boot partition (SDCARD2) 
### OS Image
[Raspbian Buster Lite -  2019-07-10](https://downloads.raspberrypi.org/raspbian_lite_latest)

## Steps for install and connect to Raspberry
### Step 1
Install the operative system in the sd card with Etcher. (SDCARD1)
### Step 2
Config raspberry pi to enable some settings like ssh. Make a blank file without extension with the name 'ssh'.
### Step 3
Connect to Raspberry with ssh client like putty (Windows) or ssh cli terminal client (Linux).

## Steps for boot Up Raspberry Pi 3 from External Hard Disk

### Step 3
- 'fdisk' to format a partition
- check partuid with 'blkid'
- https://www.maketecheasier.com/boot-up-raspberry-pi-3-external-hard-disk/
- Connect USB to raspberry
- Connect to raspberry pi
- 'df' to check partition table
- Swap file on USB
- https://www.youtube.com/watch?v=tVfMNI3w6Dw&t=664s
- but make swapon with UUID because the partition name maybe change in boot
### 

### Step 3
Install docker on raspberry


## URL
- https://www.raspberrypi.org/downloads/raspbian/
- https://www.raspberrypi.org/documentation/remote-access/ssh/ 
- https://www.raspberrypi.org/documentation/configuration/security.md
- https://opensource.com/article/18/7/how-check-free-disk-space-linux


