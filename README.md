# aa-slock
## Basically vanilla slock with just the message patch

* Run by sxhkd on `mod4+l`
* User and Group are set to `nobody` because of security reasons.
* Group is `nobody` instead of `nogroup` because Arch uses `nobody` instead.
* If failure to run, you should first change `static const char *group = "nobody"` to `static const char *group = "nogroup"` if you are not on Arch or Arch based distro.

Old, default README:
```
slock - simple screen locker
============================
simple screen locker utility for X.


Requirements
------------
In order to build slock you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (slock is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install slock
(if necessary as root):

    make clean install


Running slock
-------------
Simply invoke the 'slock' command. To get out of it, enter your password.
```
