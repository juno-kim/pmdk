# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2016, Intel Corporation

#
# examples/libpmemblk/Makefile -- build the libpmemblk examples
#
PROGS = manpage async
DIRS = assetdb

LIBS = -lpmemblk -lpmem -pthread

include ../Makefile.inc

INCS += -I/home/junokim/async_runtime/include

manpage: manpage.o

async: async.o
