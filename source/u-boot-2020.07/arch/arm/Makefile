# SPDX-License-Identifier: GPL-2.0+

# This selects which instruction set is used.
arch-$(CONFIG_CPU_ARM926EJS)	=-march=armv5te

arch-y += -D__LINUX_ARM_ARCH__=$(CONFIG_SYS_ARM_ARCH)

# Evaluate arch cc-option calls now
arch-y := $(arch-y)

# This selects how we optimise for the processor.
tune-$(CONFIG_CPU_ARM926EJS)	=

# Evaluate tune cc-option calls now
tune-y := $(tune-y)

PLATFORM_CPPFLAGS += $(arch-y) $(tune-y)

# Machine directory name.  This list is sorted alphanumerically
# by CONFIG_* macro name.
machine-$(CONFIG_ARCH_SUNXI)		+= sunxi

machdirs := $(patsubst %,arch/arm/mach-%/,$(machine-y))

PLATFORM_CPPFLAGS += $(patsubst %,-I$(srctree)/%include,$(machdirs))

libs-y += $(machdirs)

head-y := arch/arm/cpu/$(CPU)/start.o

ifeq ($(CONFIG_SPL_BUILD),y)
ifneq ($(CONFIG_SPL_START_S_PATH),)
head-y := $(CONFIG_SPL_START_S_PATH:"%"=%)/start.o
endif
endif

libs-y += arch/arm/cpu/$(CPU)/
libs-y += arch/arm/cpu/
libs-y += arch/arm/lib/

# deprecated
-include $(machdirs)/config.mk
