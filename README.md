# raspberry video loop
How to auto-play video loop on boot on Raspberry Pi

- - -

1. When Raspberry running open terminal (little icon on top left)
 
2. Type lines and always confirm with enter

`sudo apt-get update` 

`sudo apt-get install omxplayer` 

`sudo nano /etc/rc.local` 

3. Add this line at the end but before 'exit0':

`/usr/bin/omxplayer -b --loop /home/pi/Desktop/loop.mov`

`lxterminal -e omxplayer`
 
 4. Ctrl + x
 5. Confirm
 
`sudo chmod +x /etc/rc.local`

 6. Done
 
 - - - 
 
to quit video loop open terminal with shortcut: 

Ctrl + Alt + t

`killall omxplayer`
