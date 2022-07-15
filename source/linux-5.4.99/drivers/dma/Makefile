# SPDX-License-Identifier: GPL-2.0
#dmaengine debug flags
subdir-ccflags-$(CONFIG_DMADEVICES_DEBUG)  := -DDEBUG
subdir-ccflags-$(CONFIG_DMADEVICES_VDEBUG) += -DVERBOSE_DEBUG

#core
obj-$(CONFIG_DMA_ENGINE) += dmaengine.o
obj-$(CONFIG_DMA_VIRTUAL_CHANNELS) += virt-dma.o
obj-$(CONFIG_DMA_OF) += of-dma.o

#devices
obj-$(CONFIG_DMA_SUN4I) += sun4i-dma.o
