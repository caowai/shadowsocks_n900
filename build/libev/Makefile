SRCDIR=libev-4.22/

all:
	rm -rf $(SRCDIR)
	tar xvzf libev_4.22.orig.tar.gz
	cp -f ev.c $(SRCDIR)/
	@pushd $(SRCDIR)  &&\
	sh ./autogen.sh &&\
	./configure --host=arm-linux --prefix=$(INSTALL_ROOT) &&\
	make &&\
	popd;
install:
	@pushd $(SRCDIR) &&\
	make install &&\
	popd;


configflag:=$(shell echo `ls $SRCDIR/Makefile 2>/dev/null`)

clean:
ifneq ($(configflag),)
	@pushd $(SRCDIR) &&\
	make distclean &&\
	popd;
endif
	rm -rf $(SRCDIR)




