# Rtorrent + Rutorrent Auto Install Script by Patrick Kerwood


This is a Bash script i wrote to ease the installtion of rtorrent + rutorrent.

In the installation process you have to choose a system user to run rtorrent.
Also you will get the opportunity of installing 33 plugins/addons. See list further down.
The script adds a line in root's crontab, that makes rtorrent start, at
a possible reboot, in the given username's screen session.

Use rtorrent.auto.install-NEWEST-VERSION for guides or tutorials, as it will allways be the newest version.

**Installs**

This scripts installs the following packages with APT.

	openssl 
	subversion 
	apache2 
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

The script compiles and installs xmlrpc-c from svn.
Installs rtorrent-0.9.3 and libtorrent-0.13.2, downloaded at official site.
Installs rutorrent-3.5 from official site.

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
