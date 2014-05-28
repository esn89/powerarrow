Awesome Powerarrow theme for 3.5
================================

This is a fork of [Romockee's Powerarrow theme][romockee], implemented for
[Awesome-WM][awesome] 3.5 by [esn89][esn89].

**See also the [dark branch](../../tree/dark) for an alternate dark color scheme!**

Notes
-----

The enormous right-click menu from [Romockee's original][romockee] has not been
included. It is not difficult to implement, it was simply deemed unnecessary as
most people won't use the majority of it.

This fork of PowerArrow aims to be as light as possible both in terms of code
and it's desktop interface.

Installation
------------

Prerequisites:
* [Lua-oocairo](http://luaforge.net/projects/oocairo/)
  ([AUR](https://aur.archlinux.org/packages/lua-oocairo/))
* [Vicious](http://awesome.naquadah.org/wiki/Vicious)
  ([AUR](https://aur.archlinux.org/packages/vicious))

In your terminal:
* `git clone https://github.com/esn89/powerarrow.git`
* `cd powerarrow/`
* `cp -R awesome ~/.config/`

Todo:
* In the themes.lua, please change the $USER to yourself.
* In the rc.lua, change the browser and terminal to the one you are using.
* In the rc.lua at line 147, 149 change the wireless and ethernet interfaces to
  your own.  (You can find out what the name is by running `iwconfig` in your
  terminal

**Beware, some of the hotkeys/key-bindings are from my rc.lua, so if something
that you are used to pressing doesn't work, check my global keys**

What works in my version so far
-------------------------------

* The layout in general (powerline)
* Clock
* Wireless icon and data sent/received indicator (improved)
* Battery
* Volume (improved)
* CPU widget
* MEM widget
* GMail widget (improved)

(I am using wicd for my network client, if you are not using that, you should
edit out the wicd field, otherwise you will get errors)

Some differences:
-----------------

* Took out the binary clock, due to the fact that it takes me way to long to
  read.
* Added on a clock widget and icon
* Added a "netstat" drop down menu using the 'blingbling' library to indicate
  what processes are currently using the Internet
* "Sensors.lua" is not in the new Vicious library
* Volume icon instead of the core temperature.
* Working wifi-signal strength indicator.  The bars now go up or down,
  depending on your computers wifi signal strength, rather than a static icon
  that doesn't change (see screenshots for example)
* Working volume level indicated in the form of a speaker.  The icon shows the
  sound level as a speaker (see screenshots for example).
* Mail how has a notifier with gmail integration (see screenshots for example).

How to set up  gmail integration:
---------------------------------

Gmail integration:
* In your home directory, created a file named .netrc
* In this file you will put your login details, it should look like this:
  `machine mail.google.com login youremail@gmail.com password
  yoursecretpassword`  (without the quotations of course)

Future Direction:
-----------------

* Looking to implement a calendar by turning the date textbox into a button
* Will implement a battery widget that actually corresponds to the amount of
  battery you have left. (I am huge fan/advocate of icons that are dynamic, can
  change and ones that reflect on current status)
* Powerarrow dark!

Screenshots:
------------

![light theme screenshot](http://i.imgur.com/q1o4PRU.png)

![you got mail!](http://i.imgur.com/yiLCxWr.png)

![you have no mail.](http://i.imgur.com/B8gqVml.png)

![volume level high](http://i.imgur.com/80G9i0j.png)

![volume level medium](http://i.imgur.com/KdD7vNX.png)

![volume level low](http://i.imgur.com/oAiyiTi.png)

![volume icon muted](http://i.imgur.com/yaHOt3P.png)

![wifi signal low](http://i.imgur.com/oqBm8Qf.png)

![wifi signal medium](http://i.imgur.com/nb0dBOx.png)


  [awesome]: http://awesome.naquadah.org
  [esn89]: https://github.com/esn89/powerarrow
  [romockee]: https://github.com/romockee/powerarrow
