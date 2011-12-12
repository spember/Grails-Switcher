## Grails Switcher ##

Grails has frequent, active updates... faster, usually, then teams that are using the framework can safely upgrade to. If you work on several different Grails projects, it can be cumbersome switching your 'GRAILS_HOME' around to the appropriate version. Sure, many IDEs can handle the version for you if you run within the app, but if you're like me, you prefer running from the command line. I've been doing this by hand for a while now, but with the frequent 2.0 release candidates, I've worked up a little app to help me along.

Thus, the purpose of this application is to provide a quick method for switching your Grails versions.

gswitch assumes that a user has several Grails versions saved in one folder

### Requirements ###
* Groovy version 1.x
* Developed and tested on Mac OS X (Lion), thus it may work on *nix systems, but not on Windows


### Installation ###

* Export the repo such that the 'gswitch' script is somewhere in your PATH, and mark it as executable. 
* Ensure that you have GRAILS_HOME and GRAILS_PATH environment variables set. GRAILS_HOME points to your current Grails version's folder, while GRAILS_PATH points to the folder contain your Grails versions.


### Usage ###

Simply call the 'gswitch' command to view a list of your available versions:

	$ ./gswitch
	Valid versions:

	1.1
	1.1.1
	1.1.2
	1.2-M4
	1.2.0
	1.2.1
	1.3.1
	1.3.5
	1.3.7
	2.0.0.RC3

To set a version, call gswitch with a version number as the first argument. Thus, to switch to v 2.0, RC 3, type:

	./gswitch 2.0.0.RC3


