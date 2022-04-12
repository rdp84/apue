# Makefile for ids
ROOT   = ../..
CC     = gcc
CFLAGS = -Wall
EFILE  = $(ROOT)/bin/ids
INCLS  = -I$(ROOT)/include
OBJS   = ids.o

$(EFILE): $(OBJS)
		$(CC) $(CFLAGS) -o $(EFILE) $(OBJS)
$(OBJS): $(ROOT)/include/apue.h
		$(CC) $(CFLAGS) $(INCLS) -c $*.c
clean:
		rm $(EFILE) $(OBJS)
