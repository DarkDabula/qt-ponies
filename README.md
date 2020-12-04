qt-ponies
=========

Qt-ponies (pronounced 'cute-ponies') is an implementation of DesktopPonies (http://desktopponies.bugs3.com/) in Qt.
All pony data (images, behaviors, sounds) is taken from DesktopPonies, and is compatible with it.

* Based of a fork by https://github.com/orangecms/qt-ponies
* Original work of https://github.com/myszha/qt-ponies
* Inspired by qponies project by svenstaro (https://github.com/svenstaro/qponies).

Installation
------------
No precompiled packages available yet for this fork. May come soon, or not.

Building
--------
A compiler supporting C++11 (g++ >= 4.6, clang >= 3.1) is required, as are Qt (version = 5.1) libraries (and X11 developement libraries on X11 sytems).

Under Debian/Ubuntu you can install the dependencies by invoking:

    # sudo apt-get install build-essential libx11-dev libxfixes-dev libqtcore4 libqtgui4 libqt4-dev qt4-qmake

Then build qt-ponies by invoking:

    # git clone https://github.com/DarkDabula/qt-ponies
    # cd qt-ponies
    # qmake  
    # make  

Running
-------
Run 'qt-ponies'. If you have not added any ponies, the configuration window
will be shown (as is the case at first startup).

To open the configuration window, you can double-click on the system tray 
icon or right-click it and choose 'Open configuration'. You can also close
the appliacation from this menu.

Right clicking on a pony brings up its context menu, where you can put that
pony to sleep, remove it, or remove all instances of that pony.

Other information
-----------------
This is a work in progress.
Tested on Manjaro Linux x64, Qt 5.1, g++ 10.2.0.

Due to case-sensitivity of filenames under Unix, all 'pony.ini' files 
must be lower case. The case of .gif files in pony.ini must also be 
correct.

On Unix systems an X server supporting ARGB visuals and and a compositing 
window manager are required for transparency of pony windows. Something like
Compiz, Unity, Gnome Shell, KWin and most newer window managers support it.

**Configuration**

The configuration file is kept in:

On Unix:

    $HOME/.config/qt-ponies/qt-ponies.ini

On Windows:

    %APPDATA%\qt-ponies\qt-ponies.ini


Screenshots of the configuration window
---------------------------------------

* Add pony screen
 
![](http://i.imgur.com/cObuc.png)


* Active ponies screen

![](http://i.imgur.com/rLhjM.png)
