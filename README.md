# raspberry-video-loop
How to play video on boot on Raspberry Pi

1. Open terminal 

`sudo apt-get update` 

`sudo apt-get install omxplayer` 

`sudo nano /etc/rc.local` 

2. Add at the end but before 'exit0' 

`/usr/bin/omxplayer -b --loop /home/pi/Desktop/loop.mov`
 
 3. Ctrl + x
 4. Confirm
 
`sudo chmod +x /etc/rc.local`

 5. Done
 
 - - - 
 
to quit video loop open terminal: 
1. Ctrl + Alt + t

`killall omxplayer`
