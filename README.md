Ruby-Raspberry-PI

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
_this next line command take awhile to run_
sudo apt-get upgrade 

sudo apt-get install git-core
sudo wget http://goo.gl/1BOfJ -O /usr/bin/rpi-update
sudo chmod +x /usr/bin/rpi-update
sudo rpi-update

After you complete the last update command, reboot your Pi and then run this command to view memory usage:

free -h

If all goes well, you should see something like this:
free -h

Total used free shared buffers cached
Mem: 438M 98M 339M 0B 21M 40M
-/+ buffers/cache: 36M 402M
Swap: 99M 0B 99M

Once you complete all the above, your OS will now be able to make full use of the board and all the RAM  and we can start on setting up the Ruby on Rails on your Raspberry PI device.

Getting Ruby on Rails to run on Raspberry PI device

This is where I will put notes on how to get Ruby on Rails to run on Raspberry_PI

Be sure to use a good fast SC memory card, if you look at the SD card you will notice a Class 4 or Class 8 which is really common. I would recommend you find a Class 10 memory card, if you plan to do any services like media stream, RubyOnRails, Apache Web, ect. I would recommend you find a Class 10 or better memory card.

I am doing testing on a 512mRAM, ModelB, Raspberry_PI unit

I have had some problems with memory, be sure you use the command 'free -h' it will show you the memory avaiable and used. Also you want to be sure you have your updates installed so be sure to run 'sudo apt-get update' so you have all your system updated installed.

Once you get your SD Ram setup the way you want be sure to make a copy and put into an image then place in a safe location, put it up on GitHub and share with everyone else. I will have an \images folder so you can look there to see what I have been able to get working.

Best wishes, happy coding, pull and update as you see errors in my write-up, thanks in advance.

Roger Swanson Charleston, SC http://rogerswanson.me http://cneworks.com Twitter: @roger_swanson

