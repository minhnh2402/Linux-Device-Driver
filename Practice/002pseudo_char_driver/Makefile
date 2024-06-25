obj-m := main.o

ARCH=arm 
CROSS_COMPILE=arm-linux-gnueabihf-
BB_DIR=/lib/modules/6.1.33/build

all:
	make ARCH=$(ARCH) CROSS_COMPILE=$(CROSS_COMPILE) -C $(BB_DIR) M=$(PWD) modules

clean:
	make ARCH=$(ARCH) CROSS_COMPILE=$(CROSS_COMPILE) -C $(BB_DIR) M=$(PWD) clean

help:
	make ARCH=$(ARCH) CROSS_COMPILE=$(CROSS_COMPILE) -C $(BB_DIR) M=$(PWD) help

