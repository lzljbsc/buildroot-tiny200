# SPDX-License-Identifier: GPL-2.0+
#
# (C) Copyright 2000-2007
# Wolfgang Denk, DENX Software Engineering, wd@denx.de.

# There are many options which enable SPI, so make this library available
ifdef CONFIG_DM_SPI
obj-y += spi-uclass.o
obj-$(CONFIG_SPI_MEM) += spi-mem.o
else
obj-y += spi.o
endif

obj-$(CONFIG_SPI_SUNXI) += spi-sunxi.o
