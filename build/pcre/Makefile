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


configflag:=$(shell echo `ls $SRCDIR/Makefile 2>/dev/null`)

clean:
ifneq ($(configflag),)
	@pushd $(SRCDIR) &&\
	make distclean &&\
	popd;
endif
	rm -rf $(SRCDIR)




