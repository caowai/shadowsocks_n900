SRCDIR=mbedtls-2.16.1

all:
	rm -rf $(SRCDIR)
	tar xvzf mbedtls-2.16.1-apache.tgz
	mkdir -p build
	@pushd build &&\
	cmake -DCMAKE_INSTALL_PREFIX=$(INSTALL_ROOT) -DUSE_SHARED_MBEDTLS_LIBRARY=ON -DENABLE_PROGRAMS=OFF ../$(SRCDIR) &&\
	make &&\
	popd;
install:
	@pushd build &&\
	make install &&\
	popd;

clean:
	rm -rf build $(SRCDIR)




