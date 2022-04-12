# Makefile for my_shell
ROOT   = ../../..
CC     = gcc
CFLAGS = -Wall
EFILE  = $(ROOT)/bin/my_shell
INCLS  = -I$(ROOT)/include
LDDIR  = $(ROOT)/lib
OBJS   = my_shell.o $(LDDIR)/error.o

$(EFILE): $(OBJS)
		$(CC) $(CFLAGS) -o $(EFILE) $(OBJS)
$(OBJS): $(ROOT)/include/apue.h
		$(CC) $(CFLAGS) $(INCLS) -c $*.c -o $@
clean:
		rm $(EFILE) $(OBJS)
