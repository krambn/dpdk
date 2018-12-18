# SPDX-License-Identifier: BSD-3-Clause
# Copyright(c) 2016 Intel Corporation

include $(RTE_SDK)/mk/rte.vars.mk

ifeq ($(CONFIG_RTE_LIBRTE_DPDKCAP),y)

APP = dpdkcap

CFLAGS += -DALLOW_EXPERIMENTAL_API
CFLAGS += $(WERROR_FLAGS)
LDLIBS += -lncurses

# all source are stored in SRCS-y

SRCS-y := dpdkcap.c core_write.c core_capture.c statistics_ncurses.c pcap.c utils.c lzo/minilzo/minilzo.c lzo/lzowrite.c

include $(RTE_SDK)/mk/rte.app.mk

endif
