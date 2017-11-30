# stretch_right_click
Right click for touchscreen on Raspbian stretch
Python Touchscreen Right Click

This project implements right click functionality using a touchscreen on an Raspbian Stretch system using the evdev library. Because of unity's deep integration with multitouch gestures, it disallows many other systems from implementing basic gestures that are missing from the default multitouch gestures. This script will not override unity's gestures, but fill in some missing ones, working alongside unity's multitouch system.

2 finger tap Setting up script

Change directory:

cd /

Clone repository:

sudo git clone https://github.com/HM-IHL/stretch_right_click.git

Change Directory:

cd stretch_right_click

Now you can run the software:

sudo python rightclick.py

Optional: To make the code run at boot up, add to rc.local

Edit rc.local:

sudo nano /etc/rc.local

Add the following line before exit 0:

sudo python /stretch_right_click/rightclick.py

Reboot the Pi:

sudo reboot
