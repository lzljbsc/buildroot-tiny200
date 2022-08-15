# SPDX-License-Identifier: GPL-2.0+

obj-$(CONFIG_$(SPL_TPL_)CACHE) += cache/
obj-$(CONFIG_$(SPL_TPL_)CLK) += clk/
obj-$(CONFIG_$(SPL_TPL_)DM) += core/
obj-$(CONFIG_$(SPL_TPL_)DFU) += dfu/
obj-$(CONFIG_$(SPL_TPL_)GPIO_SUPPORT) += gpio/
obj-$(CONFIG_$(SPL_TPL_)INPUT) += input/
obj-$(CONFIG_$(SPL_TPL_)MMC_SUPPORT) += mmc/
obj-y += mtd/
obj-$(CONFIG_$(SPL_TPL_)PHY) += phy/
obj-$(CONFIG_$(SPL_TPL_)RTC_SUPPORT) += rtc/
obj-$(CONFIG_$(SPL_TPL_)SERIAL_SUPPORT) += serial/
obj-$(CONFIG_$(SPL_TPL_)SPI_SUPPORT) += spi/
obj-$(CONFIG_$(SPL_)BOARD) += board/

ifndef CONFIG_TPL_BUILD
ifdef CONFIG_SPL_BUILD

obj-$(CONFIG_SPL_CACHE_SUPPORT) += cache/
obj-$(CONFIG_SPL_CPU_SUPPORT) += cpu/
obj-$(CONFIG_SPL_CRYPTO_SUPPORT) += crypto/
obj-$(CONFIG_SPL_DM_RESET) += reset/
obj-$(CONFIG_SPL_MUSB_NEW_SUPPORT) += usb/musb-new/
obj-$(CONFIG_SPL_USB_GADGET) += usb/gadget/
obj-$(CONFIG_SPL_USB_GADGET) += usb/common/
obj-$(CONFIG_SPL_USB_GADGET) += usb/gadget/udc/
obj-$(CONFIG_SPL_USB_HOST_SUPPORT) += usb/host/
obj-$(CONFIG_OMAP_USB_PHY) += usb/phy/
obj-$(CONFIG_HAVE_BLOCK_DEVICE) += block/

endif
endif


ifeq ($(CONFIG_SPL_BUILD)$(CONFIG_TPL_BUILD),)

obj-y += block/
obj-$(CONFIG_CPU) += cpu/
obj-y += crypto/
obj-$(CONFIG_MMC) += mmc/
obj-y += dfu/
obj-y += phy/allwinner/
obj-y += rtc/
obj-y += video/
obj-y += mtd/
obj-y += reset/
obj-y += input/

obj-$(CONFIG_MACH_PIC32) += ddr/microchip/
endif

