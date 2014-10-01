Awesome Powerarrow theme for 3.5
================================

:Original Project: https://github.com/romockee/powerarrow

This is a fork of Romockee's Powerarrow theme, implemented
for Awesome-WM 3.5 on a Retina Apple Macbook

Notes
-----

Change the Xorg Dpi for Terminal & other in .Xressources
>  Xft.dpi:       160

Installation
------------

Lua-oocairo:
https://aur.archlinux.org/packages/lua-oocairo/

Vicious:
http://awesome.naquadah.org/wiki/Vicious#Getting_Vicious

If you are running Arch, I highly recommend you grab all that from
the repository.

In your terminal:
- ``git clone https://github.com/esn89/powerarrow.git``
- ``cd powerarrow/``
- ``cp -R awesome ~/.config/``

Todo:
- In the themes.lua, please change the $USER to yourself.
- In the rc.lua, change the browser and terminal to the one you are using.
- In the rc.lua at line 147, 149 change the wireless and ethernet interfaces to your own.  (You can find out what the name is by running ``iwconfig`` in your terminal

**Beware, some of the hotkeys/key-bindings are not yet working**


- The layout in general (powerline)
- Clock
- Wireless icon and data sent/received indicator (improved)
- Battery
- Volume (improved)
- CPU widget
- MEM widget
- GMail widget (improved)


(I am using wicd for my network client, if you are not using
that, you should edit out the wicd field, otherwise you will
get errors)

Some differences:
----------------

- Took out the binary clock, due to the fact that it takes me way to long to read.
- Added on a clock widget and icon
- Added a "netstat" drop down menu using the 'blingbling' library to indicate what processes are currently using the Internet
- "Sensors.lua" is not in the new Vicious library
- Volume icon instead of the core temperature.
- Working wifi-signal strength indicator.  The bars now go
  up or down, depending on your computers wifi signal strength, rather than a static icon that doesn't change (see screenshots for example)
- Working volume level indicated in the form of a speaker.
  The icon shows the sound level as a speaker (see
  screenshots for example).
- Mail how has a notifier with gmail integration
  (see screenshots for example).

How to set up  gmail integration:
-----------------------------------------

Gmail integration:
*****
- In your home directory, created a file named .netrc
- In this file you will put your login details, it should
look like this:
``machine mail.google.com login youremail@gmail.com password
yoursecretpassword``  (without the quotations of course)


