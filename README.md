Window Manager Scripts
======================

A series of WM agnostic shell scripts.

Maintainer Status
-----------------

(23/11/2016)

I am no longer maintaining these scripts. Feel free to fork.

About
-----

As a user of WindowMaker for almost a year, I missed some features of
desktop environments like KDE. Window Managers are small but extremely
customizable pieces of software, and the lack of certain features are due to
speed and simplicity. With these scripts, I hope to fill in the gaps someone
may feel when using something like WindowMaker or FVWM.

Scripts
-------

The following scripts are included (not all are currently finished):

- batterylow: When launched, gives a notification and plays a sound (if the 
  user desires). Intended to be used with a third party tool. Features 
  include setting xblacklight to any desired variable. Perhaps in the 
  future it will be more complex and run in the background rather than be 
  dependent on another program or applet.

- dialogsounds: Very hacky and WIP idea to play sounds via the active 
  window title when it pops up. Any better solutions are welcomed, as this 
  will have a lot of problems in theory.

- importadvanced: Screenshot tool that utilizes ImageMagick's 
  "import". Features prefix naming, date/time, parameters, format choice, 
  and FTP/SFTP uploading with clipboard. Can be configured to support 
  GraphicsMagick's command line tool instead.

- timer-xy: When launched, gives a notification that tells the user when it 
  went off and plays a sound. Intended to be used with a third party 
  program (like wmtimer). Perhaps will become more independent over time.

- videobackground: Handy for making a video play all the time as a desktop 
  background (similar to Windows DreamScene). Can be customized to use a 
  video player with any parameters. See the [wiki page] [wiki1] on how it 
  can be setup in WindowMaker and feel nicely integrated.

[wiki1]: https://github.com/Xylemon/Window-Manager-Scripts/wiki/Integrating-Videobackground-with-WindowMaker

Installation
------------

The scripts can be installed in "/usr/bin" or placed wherever you desire
(but "/usr/bin" is my recommendation).

".xyscripts" should be placed in your home folder. You'll need to go through
and edit the file to customize it for your system and setup.

Issues
------

See https://github.com/Xylemon/Window-Manager-Scripts/issues

Dependencies
------------

Required:

- Bash (at least that's what I've written these to use)
- cURL
- ImageMagick or GraphicsMagick (for importadvanced)
- Linux or Unix based systems
- xwinwrap (for videobackground)

Optional:

- A libnotify based notification daemon
- xclip if you want to use the upload URL to clipboard feature
- cURL with OpenSSL support (if you want to upload with SFTP)


License
-------

I've chosen to license all code under Public Domain, since I don't feel
anything here is deserving of a special license like GPL. Feel free to
do whatever you desire with the scripts!