# SPDX-License-Identifier: GPL-2.0+
#
# (C) Copyright 2012 Henrik Nordstrom <henrik@henriknordstrom.net>
#
# Based on some other Makefile
# (C) Copyright 2000-2003
# Wolfgang Denk, DENX Software Engineering, wd@denx.de.

obj-y	+= board.o
obj-y	+= clock.o
obj-y	+= cpu_info.o
obj-y	+= dram_helpers.o
obj-y	+= pinmux.o
obj-$(CONFIG_MACH_SUNIV)	+= clock_sun6i.o

ifdef CONFIG_SPL_BUILD
obj-$(CONFIG_MACH_SUNIV)	+= dram_suniv.o
endif
