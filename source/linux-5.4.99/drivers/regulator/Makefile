# SPDX-License-Identifier: GPL-2.0
#
# Makefile for regulator drivers.
#


obj-$(CONFIG_REGULATOR) += core.o dummy.o fixed-helper.o helpers.o devres.o
obj-$(CONFIG_OF) += of_regulator.o
obj-$(CONFIG_REGULATOR_FIXED_VOLTAGE) += fixed.o

ccflags-$(CONFIG_REGULATOR_DEBUG) += -DDEBUG
