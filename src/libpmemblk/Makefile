# SPDX-License-Identifier: BSD-3-Clause
# Copyright 2014-2020, Intel Corporation

#
# src/libpmemblk/Makefile -- Makefile for libpmemblk
#

LIBRARY_NAME = pmemblk
LIBRARY_SO_VERSION = 1
LIBRARY_VERSION = 0.0

include ../core/pmemcore.inc
include ../common/pmemcommon.inc
SOURCE +=\
	blk.c\
	btt.c\
	libpmemblk.c

include ../Makefile.inc

CFLAGS += $(LIBNDCTL_CFLAGS)
LIBS += -pthread -lpmem $(LIBNDCTL_LIBS)

# Async runtime
ASYNC_RUNTIME_ROOT = /home/junokim/async_runtime
CFLAGS += -I$(ASYNC_RUNTIME_ROOT)/include
LDFLAGS +=
LIBS +=

# DML
DML_ROOT = $(ASYNC_RUNTIME_ROOT)/dml
CFLAGS += -I$(DML_ROOT)/include
LDFLAGS += -L$(DML_ROOT)/build
LIBS += -l:libdml.a
