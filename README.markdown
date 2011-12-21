## Grails Switcher ##

Grails has frequent, active updates... faster, usually, then teams that are using the framework can safely upgrade to. If you work on several different Grails projects, it can be cumbersome switching your 'GRAILS_HOME' around to the appropriate version. Sure, many IDEs can handle the version for you if you run within the app, but if you're like me, you prefer running from the command line. I've been doing this by hand for a while now, but with the frequent 2.0 release candidates, I've worked up a little app to help me along.

Thus, the purpose of this application is to provide a quick method for switching and managing your Grails versions.

You can use gswitch to install Grails versions and switch between your active installation.


### Requirements ###
* Groovy version 1.x
* Developed and tested on Mac OS X (Lion), thus it may work on *nix systems, but not on Windows


### Installation ###

* Export the repo such that the 'gswitch' script is somewhere in your PATH, and mark it as executable. 
* Set GRAILS_HOME to be "~/.gswitch/grails" and add $GRAILS_HOME/bin to your path. The reason for this is that gswitch will create a hidden folder in your home called '.gswitch' and use a symlink to specify the current Grails version.



### Usage ###

To install a new version of Grails:

	./gswitch --install <version>

e.g.:

	./gswitch --install 2.0.0

Once installed, you can set the current version by:

	./gswitch <version>

And can list the currently installed versions by typing:

	./gswitch --versions






