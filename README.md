#Introduction

Sometimes we have to work under various network environments. At different clients, in office, at home... Switching proxy settings again and again is really annoying.

TinySwitch could help us to switch proxy setting easily.

Tinyproxy will work as a transparent proxy forwarding service. So tinyproxy is required to be installed.

Currently tinyswitch has only a CLI. 

#Requirements

    python 2.6+
    tinyproxy 


#Installation

 1. install tinyproxy if you haven't done it yet.
 2. configurate tinyproxy to make localhost:port your system proxy. And set this proxy to any of your applications that need to configurate a proxy server.
 3. download and extract the archive.

		sudo python setup.py install

 4. start application by typing `tinyswitch`, then follow the configuration wizard.
 5. `tinyswith -h` will print help information

#Usage

	 tinyswitch is tinyproxy based proxy switcher
		Usage tinyswitch [Option]
		
		OPTION 

			-v version
			-r reconfig tinyswitch
			-d delete a proxy entry from tinyswitch
			-a add a new proxy entry 
			-l list all proxy entries managed by tinyswitch
			-s [name] set/(switch to) another proxy as system proxy server (root permission needed). 
			   If [name] is given, tinyproxy will set the [name] proxy as system proxy, otherwise proxy will be set interactively.
			-h print help message

