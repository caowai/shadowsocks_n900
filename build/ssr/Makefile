SRCDIR=shadowsocks-libev

all:	
	@pushd $(SRCDIR)  &&\
	./configure  --host=arm-linux --prefix=$(INSTALL_ROOT) --disable-ssp --with-pcre=$(INSTALL_ROOT) --with-mbedtls=$(INSTALL_ROOT)--with-sodium=$(INSTALL_ROOT) CC=/scratchbox/compilers/arm-linux-cs2010q1-202/bin/arm-none-linux-gnueabi-gcc CXX=/scratchbox/compilers/arm-linux-cs2010q1-202/bin/arm-none-linux-gnueabi-g++&&\
	make &&\
	popd;
install:
	@pushd $(SRCDIR) &&\
	make install &&\
	popd;


configflag:=$(shell echo `ls shadowsocks-libev/Makefile 2>/dev/null`)

clean:
ifneq ($(configflag),)
	@pushd $(SRCDIR) &&\
	make distclean &&\
	popd;
endif


