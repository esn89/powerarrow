Awesome Powerarrow theme for 3.5
================================

:Original project: https://github.com/romockee/powerarrow
:Lots of improvements: https://github.com/esn89/powerarrow

**See also the dark branch!**

This is a fork of Romockee's Powerarrow theme, implemented for Awesome-WM 3.5. 
This project is now in a stage where 90% of the widgets work.

Notes
-----

I did not include the enormous right-click
menu that Romockee has.  Not because it is difficult to
implement, but the fact that I don't have/need 99% of the
software, books and applications he had.  If you need it, I
will be more than happy to figure it out for you.

In addition, I am trying to make this version of PowerArrow
as light as possible in terms of code and the desktop
itself.

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

**Beware, some of the hotkeys/key-bindings are from my rc.lua, so if something that you are used to pressing doesn't work, check my global keys**


What works in my version so far
-------------------------------

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

Future Direction:
-------------------------------

- Looking to implement a calendar by turning the date
  textbox into a button
- Will implement a battery widget that actually corresponds
  to the amount of battery you have left. (I am huge
  fan/advocate of icons that are dynamic, can change and
  ones that reflect on current status)
- Powerarrow dark!

Screenshots:
-------------------------------

.. image:: http://i.imgur.com/yiLCxWr.png
- you got mail!

.. image:: http://i.imgur.com/B8gqVml.png
- you have no mail.

.. image:: http://i.imgur.com/80G9i0j.png
- volume level high

.. image:: http://i.imgur.com/KdD7vNX.png
- volume level medium

.. image:: http://i.imgur.com/oAiyiTi.png
- volume level low

.. image:: http://i.imgur.com/yaHOt3P.png
- volume icon muted

.. image:: http://i.imgur.com/oqBm8Qf.png
- wifi signal low

.. image:: http://i.imgur.com/nb0dBOx.png
- wifi signal medium

.. image:: http://i.imgur.com/q1o4PRU.png
- The desktop so far
