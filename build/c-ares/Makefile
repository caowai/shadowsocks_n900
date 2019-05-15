#2019.05.15 Created by caowai (caowai@gmail.com) to build shadowsocks-libev for Nokia N900 Device

SRCDIR=c-ares-1.14.0

all:
	rm -rf $(SRCDIR)
	tar xvzf c-ares_1.14.0.orig.tar.gz
	@pushd $(SRCDIR)  &&\
	./configure --host=arm-linux --prefix=$(INSTALL_ROOT) &&\
	make &&\
	popd;
install:
	@pushd $(SRCDIR) &&\
	make install &&\
	popd;




clean:
	rm -rf $(SRCDIR)




