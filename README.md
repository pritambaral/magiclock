MagicLock
=================

A script to unlock/lock one's screen using a pre-authenticated USB Drive.

Developed by [Chhatoi Pritam Baral](http://pritambaral.com) and [Rahil Momin](http://facebook.com/rahil.rules.you)


Hack Night Competition - 2012, IIT Bombay
-----------
This application was developed in Hack Night Competition organized by [Web and Coding Club](http://stab-iitb.org/wncc). To know about other applications developed in Hack Night visit [Web and Coding Club at GitHub](https://github.com/wncc)

You can visit Web and Coding Club on [WnCC Wiki](http://stab-iitb.org/wiki/Web_n_Coding_club)

If you are IIT Bombay student then you can join [WnCC Google Group](https://groups.google.com/group/wncc_iitb)


Dependency
-----------

It depends on udisks, dbus, python-dbus, python-gobject, and python-tk for the gui. Python2 only.

To install dependecies on an Ubuntu machine run the following commands in terminal:

* sudo apt-get install python-tk python-dbus

The other dependencies should be installed by default. If not, it's time to get a proper distro. :P




Installation
----------

Clone the repository or download the zip file from [Github Repository](https://github.com/pritambaral/magiclock).

Install all the dependecies as mentioned above

To install :

* ./install.sh

To uninstall :

* ./uninstall.sh


Features and Getting Started With
-----------

Just place the two scripts anywhere in your path and call either of the two.

Changing options is acheived through the magiclock-admin script (both GUI based and command-line)

Features:

* Use any USB Removable media as a key to your workstation! (Got any broken Pen Drives lying around?)

* Convenience! No need to type in the extra-long password everytime (Especially if one is a security freak!)

* Also, no need to tell the script your system password (unlike some similar Windows tools :P )

* Just set the key, add the script to your DE's autostart list and forget about it


Insights of Define Lens
-------

The script uses DBus to listen for UDisks signals when a device is either added or removed

Locking and Unlocking is achieved by DE provided mechanisms, thus it is extensible/flexible for any compliant DE. (All freedesktop ScreenSaver specification compliant DE's work OOTB)


Advanced Usage
-------

magiclock-admin -h explains the usage

USAGE: magiclock-admin [-s SERIAL] [-l LOCKING MODE]

where SERIAL is the manufacturer serial of the device you want to use as key. LOCKING MODE is 0 for two-way operation, 1 for unlocking only.

upon successful exit, magiclock-admin restarts/starts the magiclock script in the background

USAGE: magiclock [-k]

-k kills the current running magiclock process

Authors
-------

**Chhatoi Pritam Baral**

**Department of Aerospace Engineering**

**Indian Institute of Technology, Bombay**

+ http://pritambaral.com
+ http://facebook.com/pritambaral

**Rahil Momin**

**Department of Civil Engineering**

**Indian Institute of Technology, Bombay**

+ http://facebook.com/rahil.rules.you


Copyright and license
---------------------

Copyright 2012 Chhatoi Pritam Baral <pritam@pritambaral.com>

Copyright 2012 Rahil Momin <rahil.rules.you@gmail.com>

License: [WTFPL](http://sam.zoy.org/wtfpl/)
