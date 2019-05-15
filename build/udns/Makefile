SRCDIR=udns-0.4
all:
	@pushd $(SRCDIR)  &&\
	make CC=$(CC)&&\
	popd;
install:
	@pushd $(SRCDIR) &&\
	mkdir -p $(INSTALL_ROOT)/lib/ &&\
	mkdir -p $(INSTALL_ROOT)/include/ &&\
	cp -rf libudns* $(INSTALL_ROOT)/lib/ &&\
	cp -rf udns.h $(INSTALL_ROOT)/include/ &&\
	popd;
clean:
	@pushd $(SRCDIR) &&\
	make clean &&\
	popd;




