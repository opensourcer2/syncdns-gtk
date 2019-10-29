SyncDNS-GTK
=============

## Installing
### Linux
##### Dependencies
- python 2.7, GTK 3.8 or newer and [PyGObject](https://live.gnome.org/PyGObject)
- [python-gi-cairo](https://packages.debian.org/sid/python-gi-cairo),
[gir1.2-notify](https://packages.debian.org/sid/gir1.2-notify-0.7) and [gir1.2-rsvg](https://packages.debian.org/sid/gir1.2-rsvg-2.0) on debian based distros (included in PyGObject elsewhere)
- [python-dateutil](http://labix.org/python-dateutil) (Python 2 version)
- [python-bcrypt](https://pypi.python.org/pypi/bcrypt/2.0.0)
- [setuptools](https://pypi.python.org/pypi/setuptools)
- [psmisc](http://psmisc.sourceforge.net) (for the `killall` command)
- [Syncthing](https://github.com/syncthing/syncthing) v0.13 or newer

##### Optional Dependencies
- libnotify for desktop notifications.
- nautilus-python, nemo-python or caja-python for filemanager integration
- [this Gnome Shell extension](https://extensions.gnome.org/extension/615/appindicator-support/), if running Gnome Shell
- [gir1.2-appindicator3](https://packages.debian.org/sid/gir1.2-appindicator3-0.1) (part of [libappindicator](https://launchpad.net/libappindicator)), if running Gnome Shell or Unity

For example, on Debian you need to first package it by running:
```
sudo apt-get install python
git clone https://github.com/opensourcer2/syncthing-gtk.git
cd syncthing-gtk
python setup.py sdist
```
Now you should have a package inside `dist` folder which you can install with `pip install <package_name>`.
```
sudo apt-get install python-pip
pip install dist/<package_name>
```

## Compiling
### Linux


##### Windows Building Dependencies _(you don't need to install these just to **run** Syncthing-GTK)_
- Python for Windows 2.7
- [PyGObject for Windows](http://sourceforge.net/projects/pygobjectwin32/) with GTK3 enabled (tested with version 3.14.0)
- [python-dateutil](http://labix.org/python-dateutil) (Python 2 version)
- [Python for Windows Extensions](http://sourceforge.net/projects/pywin32/)
- [WMI](http://timgolden.me.uk/python/wmi/index.html)
- [NSIS2](http://nsis.sourceforge.net/NSIS_2) with NSISdl, [ZipDLL](http://nsis.sourceforge.net/ZipDLL_plug-in) and [FindProcDLL](http://forums.winamp.com/showpost.php?p=2777729&postcount=8) plugins (optional, for building installer)

##### Related links
- https://syncthing.net
- https://forum.syncthing.net/t/syncthing-gtk-gui-for-syncthing-now-with-inotify-support/709
- https://forum.syncthing.net/t/lxle-a-respin-of-lubuntu-now-has-syncthing-included-by-default/1392
