BASEDIR=../../..

include $(BASEDIR)/Make.defs

###############################################################################
#
# Include standard packaging commands.

MIN_BIN 	= 
MIN_LIB 	= 
MIN_SBIN	= 
MIN_USR_BIN	= 
MIN_USR_LIB	= 
MIN_USR_SBIN	= 

NET_BIN 	= 
NET_LIB 	= 
NET_SBIN	= 
NET_USR_BIN	= 
NET_USR_LIB	= 
NET_USR_SBIN	= 

STD_BIN 	= 
STD_LIB 	= 
STD_SBIN	= 
STD_USR_BIN	= 
STD_USR_LIB	= 
STD_USR_SBIN	= echo_server echo_client

include $(BASEDIR)/Make.rules

###############################################################################

PRGS=echo_server echo_client

SPRGS=

all: $(PRGS)

max_rfs: install

rfs:

net_rfs: install

min_rfs:

smin_rfs:

install: all
	cp -p $(PRGS) $(TARGET_MNT)/bin

echo_server: echo_server.o

echo_client: echo_client.o

clean:
	rm -f core *.o $(PRGS)
