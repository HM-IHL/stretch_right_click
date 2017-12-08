# stretch_right_click
Right click for touchscreen on Raspbian stretch

This project implements right click functionality using a touchscreen on an Raspbian Stretch system using the evdev library. Because of unity's deep integration with multitouch gestures, it disallows many other systems from implementing basic gestures that are missing from the default multitouch gestures. This script will not override unity's gestures, but fill in some missing ones, working alongside unity's multitouch system.

2 finger tap Setting up script

install Dependencies:

*sudo apt-get install libts-bin evtest xinput python-dev python-pip*

then:

*sudo pip install pyuserinput*

then:

*sudo pip install evdev*

Change directory:

cd /

Clone repository:

sudo git clone https://github.com/HM-IHL/stretch_right_click.git

Change Directory:

cd stretch_right_click

Copy files to the correct directories:

sudo cp profile /etc/profile

this will allow you to reboot the pi and have the software setup for you

Reboot the Pi:

sudo reboot

Note: if the right click doesnt work, then run the following line to see which devices are available:

ls /dev/input/event*

then change line 15 with the corrent event number.
