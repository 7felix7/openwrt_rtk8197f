# Realtek Semiconductor Corp.
#
# bsp/Makefile
#     bsp Makefile
#
# Copyright (C) 2006-2012 Tony Wu (tonywu@realtek.com)
#


# mips-ori
#core-y   += arch/mips/bsp/
#cflags-y += -Iinclude/asm-mips -Iarch/mips/bsp/
#load-y   += 0x80000000

obj-y := prom.o setup.o irq.o timer.o serial.o
obj-$(CONFIG_PCI) += pci-fixup.o pci-ops.o
#obj-$(CONFIG_PCI) += pci.o
obj-$(CONFIG_RTL_819X) += pci.o
obj-$(CONFIG_USB) += dev_usb.o
obj-$(CONFIG_SPI_SHEIPA) += mtd.o
#obj-$(CONFIG_RTL819X_GPIO) += gpio.o
obj-$(CONFIG_GPIOLIB) += gpio.o dev-gpio-buttons.o mach_rtl819x.o
obj-$(CONFIG_LEDS_GPIO) += dev_leds_gpio.o

