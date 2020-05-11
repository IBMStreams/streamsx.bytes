#######################################################################
# Copyright (C)2020, International Business Machines Corporation and
# others. All Rights Reserved.
#######################################################################


.PHONY: all distributed clean 

SPLC_FLAGS = -a -t ../../com.ibm.streamsx.bytes
SPLC = $(STREAMS_INSTALL)/bin/sc
SPL_CMD_ARGS ?= 
SPL_MAIN_COMPOSITE = com.ibm.streamsx.bytes.sample::Ais

all: distributed

distributed:
	$(SPLC) $(SPLC_FLAGS) -M $(SPL_MAIN_COMPOSITE) $(SPL_CMD_ARGS)

clean: 
	$(SPLC) $(SPLC_FLAGS) -C -M $(SPL_MAIN_COMPOSITE)

