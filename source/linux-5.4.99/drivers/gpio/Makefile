# SPDX-License-Identifier: GPL-2.0
# generic gpio support: platform drivers, dedicated expander chips, etc

ccflags-$(CONFIG_DEBUG_GPIO)	+= -DDEBUG

obj-$(CONFIG_GPIOLIB)		+= gpiolib.o
obj-$(CONFIG_GPIOLIB)		+= gpiolib-devres.o
obj-$(CONFIG_GPIOLIB)		+= gpiolib-legacy.o
obj-$(CONFIG_GPIOLIB)		+= gpiolib-devprop.o
obj-$(CONFIG_OF_GPIO)		+= gpiolib-of.o
obj-$(CONFIG_GPIO_SYSFS)	+= gpiolib-sysfs.o
obj-$(CONFIG_GPIO_ACPI)		+= gpiolib-acpi.o

# Device drivers. Generally keep list sorted alphabetically
obj-$(CONFIG_GPIO_GENERIC)	+= gpio-generic.o

# directly supported by gpio-generic
gpio-generic-$(CONFIG_GPIO_GENERIC)	+= gpio-mmio.o

