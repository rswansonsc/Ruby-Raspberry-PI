Ruby-Raspberry-PI
=================

First I want to walk through getting your SD Card setup:

Next we can work on getting Ruby on Rails to run on Raspberry PI device, memory looks to be an issue so be sure to use the utility to figure out your memory.  

First Section starts here:
Setting up Raspberry PI on MacBook Air
Setup your SD Card, Here are some images and sites to help you:
http://www.raspberrypi.org/downloads/
Get an SD Card, you can follow directions on the www.raspberrypi.org site, first you will want to clean any old files off the SD Card,  if you have a memory card you want to be sure is wiped you can take a look at this site: 

There are some great instructions on the site - http://www.sdcard.org
also have a look at this site - http://www.raspberrypi.org/help/noobs-setup

Here are the instructions if you want to start from scratch: 
http://elinux.org/RPi_Ruby_on_Rails

Download the Wheezy version
Use the SD writing tool to copy *.img file to the SD Card
-copy image to SD from a file: 


Commands to help troubleshoot:
-always login user: pi
-switch to super user: sudo su
-show memory: free -htl

Update Raspberry-PI Firmware:
Log into the board via SSH or on a local keyboard and run the following commands:

sudo apt-get update 
#this next line command take awhile to run
sudo apt-get upgrade 

sudo apt-get install git-core
sudo wget http://goo.gl/1BOfJ -O /usr/bin/rpi-update
sudo chmod +x /usr/bin/rpi-update
sudo rpi-update
After you complete the last update command, reboot your Pi and then run this command to view memory usage:

free -h

If all goes well, you should see something like this:
free -h
 total used free shared buffers cached
Mem: 438M 98M 339M 0B 21M 40M
-/+ buffers/cache: 36M 402M
Swap: 99M 0B 99M

Once you complete all the above, your OS will now be able to make full use of the board and all the RAM  and we can start on setting up the Ruby on Rails on your Raspberry PI device.

