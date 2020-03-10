# raspberry video loop
How to auto-play video loop on boot on Raspberry Pi

- - -

## autoload raspberry video 
1. Reinstall OS if already on unbreakable auto-loop 
2. Place .mov or .mp4 file on desktop, in this example `loop.mov`
3. Create `autostart` folder here: `/home/pi/.config/autostart` 
4. In this `autostart` folder create a text file called `.desktop` and put in the following: 
 
```
[Desktop Entry]

Type=Application

Exec=lxterminal -e "omxplayer -b --loop --no-osd /home/pi/Desktop/loop.mov"
``` 
5. Make file executable in terminal:

`sudo chmod +x /home/pi/.config/autostart/.desktop` 
