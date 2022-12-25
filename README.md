# screenlocker
Lock the screen making a screenshot of your current desktop and blurring the entire image

# 1.Create a command at /bin/ called "lock" (so the path to the command should be /bin/lock)  
 
 *cd /bin  
 *sudo nvim lock  
   
# 2.Paste this to the file 

---------------------------------------------------
#!/bin/bash  
  
rm /tmp/screenshot.png  
scrot /tmp/screenshot.png  
betterlockscreen -u /tmp/screenshot.png -l dimblur

---------------------------------------------------
  
# 3.Enjoy
