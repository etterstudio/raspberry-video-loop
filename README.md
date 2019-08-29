# raspberry-video-loop
How to play video on boot on Raspberry Pi

1 terminal 
sudo apt-get update 
sudo apt-get install omxplayer 

sudo nano /etc/rc.local

3 Add at the end but before 'exit0' 
/usr/bin/omxplayer -b --loop /home/pi/Desktop/loop.mov
 
 Ctrl + X 
 Confirm
 
 sudo chmod +x /etc/rc.local
 
6 Done
 
7 To Exit 
Terminal: 
killall omxplayer
