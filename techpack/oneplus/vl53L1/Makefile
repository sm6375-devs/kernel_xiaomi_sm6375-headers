ifneq ($(KERNELRELEASE),)
include Kbuild

else
KDIR ?= /lib/modules/`uname -r`/build

default:
	CONFIG_STMVL53L1=y $(MAKE) -C $(KDIR) M=$$PWD
clean:
	CONFIG_STMVL53L1=y $(MAKE) -C $(KDIR) M=$$PWD clean

endif