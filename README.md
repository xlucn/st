st - simple terminal
--------------------
st is a simple terminal emulator for X which sucks less.


About this fork
---------

**NOTE**:

- I am tracking the upstream suckless code in a separate branch called 'suckless'. My commits are always on the top.
- I reorganize the commits time to time to keep things in order, so if you want to use my fork, remember to use `git pull --force` to update.

Patches and changes applied in this fork, my changes and comments see the commit messages:

- [alpha](https://st.suckless.org/patches/alpha/)
- [scrollback](https://st.suckless.org/patches/scrollback/), All the scroll patches, plus `Shift+PageUp/PageDown` to scroll *a whole page*
- [xresources](https://st.suckless.org/patches/xresources/)
- [externalpipe](https://st.suckless.org/patches/externalpipe/)
- [hidecursor](https://st.suckless.org/patches/hidecursor/)
- Added a desktop entry file
- Disabled size hint, i.e. resize by 1 pixel instead of a character
- Some customizations in config.def.h


Requirements
------------
In order to build st you need the Xlib header files.


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install


Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

