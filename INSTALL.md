Requirements
------------
- Any Linux distribution
- Gambas 3: gambas3-ide gambas3-gb-net gambas3-gb-net-curl gambas3-gb-eval-highlight gambas3-gb-gui 
- ffmpeg or libav-tools (avconv)
- git
- libnotify
- xdg-utils
- pkill (for pause functionality)
- for newer Gambas versions (~3.5+), gambas3-gb-form-editor and gambas3-gb-desktop-x11 are required

Tip: on recent Ubuntu versions:
- you can install Gambas 3 by installing the packages above.
- add the [Gambas PPA](https://launchpad.net/~gambas-team/+archive/ubuntu/gambas3): sudo add-apt-repository ppa:gambas-team/gambas
- then upgrade all installed Gambas packages: sudo apt-get install gambas3-gb-db gambas3-gb-db-form gambas3-gb-desktop gambas3-gb-eval-highlight gambas3-gb-form gambas3-gb-form-dialog gambas3-gb-form-mdi gambas3-gb-form-stock gambas3-gb-settings gambas3-ide gambas3-runtime
- and upgrade another set: sudo apt-get install gambas3-gb-gtk gambas3-gb-net gambas3-gb-net-curl gambas3-gb-qt4-ext

Please use the packages of your Linux distribution if they are available.

Optional integration components
-------------------------------
For GTK environments:
- gambas3-gb-gtk (for GTK 2 support)
- gambas3-gb-gtk3 (for GTK 3 support)
- gambas3-gb-desktop, provided by gambas3-gb-desktop-gnome

For Qt environments:
- gambas3-gb-gui-qt (for Qt support), provided by gambas3-gb-qt4
- gambas3-gb-gui-qt-webkit, provided by gambas3-gb-qt4-webkit

Recommended players:
* mpv
* VLC Media Player

Other players can be used too, but only these two support the pause mode for now.

Developer components
---------------------
gambas3-gb-util

Installation
------------
If you have not installed the required packages, do it now using your packaging manager. After installing the requirements, open a terminal window and continue with the installation:

- cd
- git clone https://github.com/Smile4ever/Text2SRT.git
- cd Text2SRT
- mkdir ~/.local/share/text2srt
- cp -r . ~/.local/share/text2srt/
- mkdir ~/.local/share/applications/
- cp desktop-integration/text2srt.desktop ~/.local/share/applications/

If you have a GTK environment and you wish to use the GTK style for Text2SRT, do this:
- cd ~/.local/share/text2srt/.src
- mv FBrowser.class FBrowser.class.backup
- mv FBrowser.form FBrowser.form.backup
- cp GtkFBrowser.class FBrowser.class
- cp GtkFBrowser.form FBrowser.form

You can now open Text2SRT from your Applications menu (category Utility).
