Random tweaks for ubuntu
=============
This is a list of tweaks that I need to run before I get Ubuntu 13.10 useful.

Keyboard Fixes
============
First things first, run theese commands to fix keyboard switching and be able to set shift+alt as a shortcut
```
  sudo add-apt-repository ppa:attente/modifier-only-input-switch
  sudo apt-get update
  sudo apt-get upgrade
```
Mouse fixes
===========
Then, we set up imwheel because I use a generic mouse

Edit ~/.imwheelrc and make it
```
".*"
None,       Up,     Up,     3
None,       Down,   Down,   3
```



Afterward, we add in /usr/bin/imwheel to the startup program list

Back Buttons
=============
I commonly use backspace as a back button. To add it to nautils, edit

~/.config/nautilus/accels


and add

     (gtk_accel_path "<Actions>/ShellActions/Up" "BackSpace")




To add it in chromium, we install

https://chrome.google.com/webstore/detail/backspace-as-backforward/aeffggjddcchloadflonilaahpclmbnm

To add it in firefox, which I often switch to, we open

about:config

and we search for

browser.backspace_action

and we set it to 0

