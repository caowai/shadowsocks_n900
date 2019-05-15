SRCDIR=libsodium-1.0.16

all:
	rm -rf $(SRCDIR)
	tar xvzf libsodium_1.0.16.orig.tar.gz
	@pushd $(SRCDIR)  &&\
	./autogen.sh &&\
	./configure --host=arm-linux --prefix=$(INSTALL_ROOT) &&\
	make &&\
	popd;
install:
	@pushd $(SRCDIR) &&\
	make install &&\
	popd;
clean:
	rm -rf $(SRCDIR)




