# SPDX-License-Identifier: GPL-2.0
#
# Makefile for kernel SPI drivers.
#

ccflags-$(CONFIG_SPI_DEBUG) := -DDEBUG

# small core, mostly translating board-specific
# config declarations into driver model code
obj-$(CONFIG_SPI_MASTER)		+= spi.o
obj-$(CONFIG_SPI_MEM)			+= spi-mem.o
obj-$(CONFIG_SPI_SPIDEV)		+= spidev.o

# SPI master controller drivers (bus)
obj-$(CONFIG_SPI_BITBANG)		+= spi-bitbang.o
obj-$(CONFIG_SPI_GPIO)			+= spi-gpio.o
obj-$(CONFIG_SPI_SUN6I)			+= spi-sun6i.o
