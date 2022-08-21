# SPDX-License-Identifier: GPL-2.0+
#
# (C) Copyright 2004-2006
# Wolfgang Denk, DENX Software Engineering, wd@denx.de.

obj-$(CONFIG_$(SPL_TPL_)ENV_SUPPORT) += common.o
obj-$(CONFIG_$(SPL_TPL_)ENV_SUPPORT) += env.o
obj-$(CONFIG_$(SPL_TPL_)ENV_SUPPORT) += attr.o
obj-$(CONFIG_$(SPL_TPL_)ENV_SUPPORT) += flags.o

ifndef CONFIG_SPL_BUILD
obj-y += callback.o
endif

obj-$(CONFIG_$(SPL_TPL_)ENV_IS_NOWHERE) += nowhere.o

CFLAGS_embedded.o := -Wa,--no-warn -DENV_CRC=$(shell tools/envcrc 2>/dev/null)
