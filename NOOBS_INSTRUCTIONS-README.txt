NOOBS INSTALLATION INSTRUCTIONS
To get these files go to this site: 

The latest official release of NOOBS can be downloaded from http://downloads.raspberrypi.org/NOOBS_latest

For information on previous releases and version change lists, visit 
https://github.com/raspberrypi/noobs/releases

1. Insert an SD card that is 4GB or greater in size into your computer.
2. Format the SD card using the platform-specific instructions below:
   a. Windows
      i. Download the SD Association's Formatting Tool from https://www.sdcard.org/downloads/formatter_4/eula_windows/
      ii. Install and run the Formatting Tool on your machine
      iii. Set "FORMAT SIZE ADJUSTMENT" option to "ON" in the "Options" menu
      iv. Check that the SD card you inserted matches the one selected by the Tool
      v. Click the "Format" button
   b. Mac
      i. Download the SD Association's Formatting Tool from https://www.sdcard.org/downloads/formatter_4/eula_mac/
      ii. Install and run the Formatting Tool on your machine
      iii. Select "Overwrite Format"
      iv. Check that the SD card you inserted matches the one selected by the Tool
      v. Click the "Format" button
   c. Linux
      i. We recommend using gparted (or the command line version parted)
      ii. Format the entire disk as FAT
3. Extract the files contained in this NOOBS zip file.
4. Copy the extracted files onto the SD card that you just formatted so that this file is at the root directory of the SD card. Please note that in some cases it may extract the files into a folder, if this is the case then please copy across the files from inside the folder rather than the folder itself.
5. Insert the SD card into your Pi and connect the power supply.

Your Pi will now boot into NOOBS and should display a list of operating systems that you can choose to install.
*****
If your display remains blank, you should select the correct output mode for your display by pressing one of the following number keys on your keyboard:
1. HDMI mode - this is the default display mode.
2. HDMI safe mode - select this mode if you are using the HDMI connector and cannot see anything on screen when the Pi has booted.
3. Composite PAL mode - select either this mode or composite NTSC mode if you are using the composite RCA video connector.
4. Composite NTSC mode

If you are still having difficulties after following these instructions, then please visit the Raspberry Pi Forum ( http://www.raspberrypi.org/phpBB3/ ) for support.
*****

When the Raspberry PI reboots you will be placed into a Raspberry PI Software Configuration Tool (raspi-config)
-do not Overclock this will void warranty and cause system to run hot and possible fail

Here is what I recommend you do:
1. first run the update tool option, (advanced options, A7)
2. expand file system, this may have already run, (main screen option, 1.)
3. advance options, give the system more RAM to run 256m is max that i found (advanced options, A3), default is 64m.
4. connect to ethernet and get on line, test connection 'ping www.goole.com'
5. give your raspberry pi a unique hostname (advanced options, A2)
6. user to login is always 'pi', default password is 'raspberry', change it.
7. change your password (write it down)(advanced options, A2), default is raspberry
8. enable SSH to remote into system using simple ssh pi@ip_address_goes_here
8a. show your ip "ifconfig"
8b. ssh pi@your_ip_address, so pi is the user, system will ask you for that password
9. run 'ruby-pi to get setup for RubyOnRails'
10. run 'ror-test-school', be sure to check the directions before you run command
11. open browser localhost:3000 (localhost is your ip address, use 'ifconfig' to get ip address)