# SPDX-License-Identifier: GPL-2.0+
#
# for USB OTG silicon based on Mentor Graphics INVENTRA designs

obj-$(CONFIG_USB_MUSB_GADGET) += musb_gadget.o musb_gadget_ep0.o musb_core.o
obj-$(CONFIG_USB_MUSB_GADGET) += musb_uboot.o
obj-$(CONFIG_USB_MUSB_SUNXI) += sunxi.o

ccflags-y := $(call cc-option,-Wno-unused-variable) \
		$(call cc-option,-Wno-unused-but-set-variable) \
		$(call cc-option,-Wno-unused-label)
