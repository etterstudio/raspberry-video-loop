# raspberry-video-loop
How to play video on boot on Raspberry Pi

1. Open terminal 
2. sudo apt-get update 
3. sudo apt-get install omxplayer 
4. sudo nano /etc/rc.local
5. Add at the end but before 'exit0' 

# /usr/bin/omxplayer -b --loop /home/pi/Desktop/loop.mov
 
 6. Ctrl + x
 7. Confirm
 8. sudo chmod +x /etc/rc.local
 9. Done
 
 - - - 
 
10. to quit video loop open terminal: 
11. Ctrl + Alt + t
12. killall omxplayer
