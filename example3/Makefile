obj-m   := my_debugfs.o
KDIR    := /lib/modules/$(shell uname -r)/build
PWD     := $(shell pwd)

all:
	$(MAKE) -C $(KDIR) SUBDIRS=$(PWD) modules

clean:
	rm -f *.o *.ko *.cmd modules.order Module.symvers *.mod.c
