target ?= test_tresor_lkm
obj-m += $(target).o


KDIR := /lib/modules/$(shell uname -r)/build

all:
	make -C $(KDIR) M=$(shell pwd) modules
	#make -C $(KDIR) M=$(shell pwd) modules_install
 
clean:
	make -C $(KDIR) M=$(shell pwd) clean
