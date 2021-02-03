all:
	tar xf freeswitch-1.10.5.-release.tar.xz
	cd freeswitch-1.10.5.-release && ./configure --prefix=/usr
	$(MAKE) -C freeswitch-1.10.5.-release
	$(MAKE) -C freeswitch-1.10.5.-release check
	$(MAKE) -C freeswitch-1.10.5.-release install
	rm -rf freeswitch-1.10.5.-release
