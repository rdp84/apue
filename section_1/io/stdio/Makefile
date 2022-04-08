# Makefile to build cp_io
ROOT   = ../../..
CC     = gcc
CFLAGS = -Wall
EFILE  = $(ROOT)/bin/cp_io
INCLS  = -I$(ROOT)/include
LDDIR  = $(ROOT)/lib
OBJS   = cp_io.o $(LDDIR)/error.o

$(EFILE): $(OBJS)
		$(CC) $(CFLAGS) -o $(EFILE) $(OBJS)
$(OBJS): $(ROOT)/include/apue.h
		$(CC) $(CFLAGS) $(INCLS) -c $*.c -o $@
clean:
		rm $(EFILE) $(OBJS)
