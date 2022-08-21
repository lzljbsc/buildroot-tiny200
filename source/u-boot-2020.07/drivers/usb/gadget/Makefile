# SPDX-License-Identifier: GPL-2.0+
#
# (C) Copyright 2000-2007
# Wolfgang Denk, DENX Software Engineering, wd@denx.de.

obj-$(CONFIG_USB_GADGET) += epautoconf.o config.o usbstring.o
obj-$(CONFIG_USB_ETHER) += epautoconf.o config.o usbstring.o

ifdef CONFIG_SPL_BUILD
obj-$(CONFIG_SPL_USB_GADGET) += g_dnl.o
obj-$(CONFIG_SPL_DFU) += f_dfu.o
endif

# new USB gadget layer dependencies
ifdef CONFIG_USB_GADGET
ifndef CONFIG_SPL_BUILD
obj-$(CONFIG_USB_GADGET_DOWNLOAD) += g_dnl.o
obj-$(CONFIG_DFU_OVER_USB) += f_dfu.o
obj-$(CONFIG_USB_FUNCTION_MASS_STORAGE) += f_mass_storage.o
endif
endif
