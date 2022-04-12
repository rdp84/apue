# Makefile for print_err
ROOT   = ../..
CC     = gcc
CFLAGS = -Wall
INCLS  = -I$(ROOT)/include
EFILE  = $(ROOT)/bin/print_err
OBJS   = print_err.o

$(EFILE): $(OBJS)
		$(CC) $(CFLAGS) -o $(EFILE) $(OBJS)
$(OBJS): $(ROOT)/include/apue.h
		$(CC) $(CFLAGS) $(INCLS) -c $*.c
clean:
		rm $(EFILE) $(OBJS)
