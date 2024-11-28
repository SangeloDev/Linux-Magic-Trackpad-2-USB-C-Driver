KERNEL_VERSION	:= $(shell uname -r)
KERNEL_MODULES	:= /lib/modules/$(KERNEL_VERSION)/build

#hid-y := hid-magicmouse_usbc.o

obj-m += hid-magicmouse_usbc.o
hid-magicmouse_usbc-objs := hid-magicmouse.o

all:
	$(MAKE) -C $(KERNEL_MODULES) M=$(PWD) modules

clean:
	$(MAKE) -C $(KERNEL_MODULES) M=$(PWD) clean
