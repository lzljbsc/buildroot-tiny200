# SPDX-License-Identifier: GPL-2.0+
#
# (C) Copyright 2000-2006
# Wolfgang Denk, DENX Software Engineering, wd@denx.de.
# Copyright (c) 2012, NVIDIA CORPORATION.  All rights reserved.

ifdef CONFIG_SPL_BUILD
obj-$(CONFIG_FS_LOADER) += fs.o
obj-$(CONFIG_SPL_FS_FAT) += fat/
obj-$(CONFIG_SPL_FS_EXT4) += ext4/
else
obj-y				+= fs.o

obj-$(CONFIG_FS_EXT4) += ext4/
obj-$(CONFIG_FS_FAT) += fat/
endif
obj-y += fs_internal.o
