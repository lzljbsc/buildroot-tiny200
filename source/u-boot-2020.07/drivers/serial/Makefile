# SPDX-License-Identifier: GPL-2.0+
#
# (C) Copyright 2006-2009
# Wolfgang Denk, DENX Software Engineering, wd@denx.de.

ifdef CONFIG_SPL_BUILD

ifeq ($(CONFIG_$(SPL_TPL_)BUILD)$(CONFIG_$(SPL_TPL_)DM_SERIAL),yy)
obj-y += serial-uclass.o
else
obj-y += serial.o
endif

else

ifdef CONFIG_DM_SERIAL
obj-y += serial-uclass.o
else
obj-y += serial.o
endif

endif

ifdef CONFIG_DM_SERIAL
else
obj-$(CONFIG_SYS_NS16550_SERIAL) += serial_ns16550.o
endif

obj-$(CONFIG_SYS_NS16550) += ns16550.o
