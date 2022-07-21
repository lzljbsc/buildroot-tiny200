# SPDX-License-Identifier: GPL-2.0
# generic pinmux support

subdir-ccflags-$(CONFIG_DEBUG_PINCTRL)	+= -DDEBUG

obj-y				+= core.o pinctrl-utils.o
obj-$(CONFIG_PINMUX)		+= pinmux.o
obj-$(CONFIG_PINCONF)		+= pinconf.o
obj-$(CONFIG_OF)		+= devicetree.o
obj-$(CONFIG_GENERIC_PINCONF)	+= pinconf-generic.o

obj-$(CONFIG_PINCTRL_SUNXI)	+= sunxi/
