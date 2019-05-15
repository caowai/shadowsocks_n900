#2019.05.15 Created by caowai (caowai@gmail.com) to build shadowsocks-libev for Nokia N900 Device
SRCDIR=pcre-8.43

all:
	rm -rf $(SRCDIR)
	tar xvzf pcre-8.43.tar.gz
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




