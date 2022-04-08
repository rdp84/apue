# Makefile to build cp_nio
ROOT   = ../../..
CC     = gcc
CFLAGS = -Wall
EFILE  = ${ROOT}/bin/cp_nio
INCLS  = -I$(ROOT)/include
LDDIR  = $(ROOT)/lib
OBJS   = cp_nio.o $(LDDIR)/error.o

$(EFILE): $(OBJS)
		$(CC) $(CFLAGS) -o $(EFILE) $(OBJS)
$(OBJS): $(ROOT)/include/apue.h
		$(CC) $(CFLAGS) $(INCLS) -c $*.c -o $@
clean:
		rm $(EFILE) $(OBJS)
