# Rtorrent + Rutorrent Auto Install Script by Patrick Kerwood

http://LinuxBloggen.dk/ 
 
 
This is a Bash script to ease the installation of rtorrent, rutorrent + plugins.

The Ubuntu 14.04 script was forked by Frantz @ [Wiity.net](http://Wiity.net), who made it run on Ubuntu, so a big thank you to him.

In the installation process you have to choose a system user to run rtorrent.
Also you will get the opportunity of installing 43 plugins/addons. See list further down.
The script add a init script that makes rtorrent start, at a possible reboot, in the 
given username's screen session. Use "service rtorrent-init start" and 
"service rtorrent-init stop" to start and stop rtorrent.


Installation
------------
 
Installation video here - https://www.youtube.com/watch?v=3iwsoKcUgn0 

Download the script. 

	wget https://raw.github.com/Kerwood/rtorrent.auto.install/master/rtorrent.auto.install-X.X.X-Debian-Wheezy

Make it executable. 

	chmod +x rtorrent.auto.install-X.X.X-Debian-Wheezy

Run the script. 

	sudo ./rtorrent.auto.install-X.X.X-Debian-Wheezy

Login box does not appear after install!!
-----------------------------------------

If the login box does not appear, it is properly because you have installed the all-plugins-pack or manually installed either `httprpc` and/or `rpc` plugins.
If one of these plugins are installed (they both are in the plugins pack), you can either remove them or manually make a .htaccess file in `/var/www/rutorrent`.

	sudo rm -rv /var/www/rutorrent/plugins/{httprpc,rpc}

Installs
--------

This scripts installs the following packages with APT.

	openssl 
	subversion
	git
	apache2
	apache2-utils 
	build-essential 
	libsigc++-2.0-dev 
	libcurl4-openssl-dev 
	automake libtool 
	libcppunit-dev 
	libncurses5-dev 
	libapache2-mod-scgi 
	php5 
	php5-curl 
	php5-cli 
	libapache2-mod-php5 
	screen
	unrar-free
	unzip

The script compiles and installs lastest xmlrpc-c from svn.  
Installs rtorrent-0.9.4 and libtorrent-0.13.4, from github.  
Installs rutorrent-3.6 from official site.

**Plugin List**

- 1 - Erase Data Plugin
- 2 - Create Plugin
- 3 - Trafic Plugin	
- 4 - RSS Plugin
- 5 - Edit Plugin
- 6 - Retrackers Plugin
- 7 - Throttle Plugin
- 8 - Cookies Plugin
- 9 - Scheduler Plugin
- 10 - Auto Tools Plugin
- 11 - Data Dir Plugin
- 12 - Track Lables Plugin 
- 13 - Geo IP Plugin
- 14 - Ratio Plugin 
- 15 - Show Peers like wTorrent Plugin
- 16 - Seeding Time Plugin 
- 17 - HTTPRPC Plugin
- 18 - Diskspace Plugin
- 19 - Unpack Plugin
- 20 - Get Dir Plugin
- 21 - Source Plugin
- 22 - Chunks Plugin
- 23 - Data Plugin
- 24 - CPU Load Plugin
- 25 - Extsearch Plugin
- 26 - Theme Plugin
- 27 - Login Mgr Plugin
- 28 - ruTorrent Label Management Suite 
- 29 - NFO Plugin
- 30 - Chat Plugin
- 31 - Logoff Plugin
- 32 - Pause Plugin
- 33 - Instant Search Plugin
- 34 - File Drop (FF > 3.6 & Chrome only).
- 35 - Check Port
- 36 - History
- 37 - iPad
- 38 - Extended Ratio
- 39 - Feeds
- 40 - Media Information
- 41 - RSS URL Rewrite
- 42 - Screenshot
- 43 - RPC
- 44 - Rutracker Check
- 45 - Noty 
- 46 - Task 
- 47 - All Plugins v3.6, Download manually to se which ones. https://bintray.com/novik65/generic/ruTorrent


