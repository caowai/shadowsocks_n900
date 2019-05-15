#2019.05.15 Created by caowai (caowai@gmail.com) to build shadowsocks-libev for Nokia N900 Device
#Please install scratchbox first

export CC = /scratchbox/compilers/cs2007q3-glibc2.5-arm7/bin/arm-none-linux-gnueabi-gcc
export CXX = /scratchbox/compilers/cs2007q3-glibc2.5-arm7/bin/arm-none-linux-gnueabi-g++
export INSTALL_ROOT = $(PWD)/target_rootfs
export LDFLAGS += -L$(INSTALL_ROOT)/lib
export CPPFLAGS += -I$(INSTALL_ROOT)/lib

#Depend third party libs 
LIBDIRS += c-ares
LIBDIRS += libev
LIBDIRS += libsodium
LIBDIRS += mbedtls
LIBDIRS += pcre
LIBDIRS += udns
#Shadowsocks-libev 
APPDIRS += ssr



all: prepare libs apps

libs: 
	for i in ${LIBDIRS}; do \
	(cd $$i; make; make install) || exit 1; \
	done

apps: 
	for i in ${APPDIRS}; do \
	(cd $$i; make; make install) || exit 1; \
	done

prepare:
	mkdir -p $(INSTALL_ROOT)

clean: 
	for i in ${LIBDIRS} ${APPDIRS}; do \
	(cd $$i; make clean) || exit 1; \
	done
	rm -rf $(INSTALL_ROOT)

%_only: prepare
	cd $(@:_only=); make
%_install:
	cd $(@:_install=); make install
%_clean:
	cd $(@:_clean=); make clean








