Requirements
------------
- Any Linux distribution
- Gambas 3: gambas-ide gambas3-gb-net gambas3-gb-net-curl gambas3-gb-net-smtp gambas3-gb-qt4 gambas3-gb-form-editor gambas3-gb-qt4-webkit gambas3-gb-eval-highlight gambas3-gb-eval
- ffmpeg or libav-tools (avconv)
- git
- libnotify
- xdg-utils
- pkill (for pause functionality)
- ~~gambas3-gb-gtk (for GTK support)~~ (cannot be used because we depend on gambas3-gb-qt4-webkit)

Recommended players:
* mpv
* VLC Media Player

Other players can be used too, but only these two support the pause mode for now.

Installation
------------
If you have not installed the required packages, do it now using your packaging manager. After installing the requirements, open a terminal window and continue with the installation:

- cd
- git clone https://github.com/Smile4ever/Text2SRT.git
- cd Text2SRT
- sudo mkdir /usr/lib/text2srt
- sudo cp -r . /usr/lib/text2srt/
- sudo cp /usr/lib/text2srt/desktop-integration/text2srt.desktop /usr/share/applications

You can now open Text2SRT from your Applications menu (category Utility).
