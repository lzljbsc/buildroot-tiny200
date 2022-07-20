# SPDX-License-Identifier: GPL-2.0
#
# Makefile for the linux networking.
#
# 2 Sep 2000, Christoph Hellwig <hch@infradead.org>
# Rewritten to use lists instead of if-statements.
#

obj-$(CONFIG_NET)		:= socket.o core/

obj-$(CONFIG_NET)		+= ethernet/ sched/ netlink/
obj-$(CONFIG_INET)		+= ipv4/
obj-$(CONFIG_UNIX_SCM)		+= unix/
obj-$(CONFIG_NET)		+= ipv6/
obj-$(CONFIG_PACKET)		+= packet/
obj-$(CONFIG_WIRELESS)		+= wireless/
obj-$(CONFIG_MAC80211)		+= mac80211/

ifeq ($(CONFIG_NET),y)
obj-$(CONFIG_SYSCTL)		+= sysctl_net.o
endif
obj-$(CONFIG_DNS_RESOLVER)	+= dns_resolver/
