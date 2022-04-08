# Makefile to print print_pid
ROOT   = ../../..
CC     = gcc
CFLAGS = -Wall
EFILE  = $(ROOT)/bin/print_pid
INCLS  = -I$(ROOT)/include
OBJS   = print_pid.o

$(EFILE): $(OBJS)
		$(CC) $(CFLAGS) -o $(EFILE) $(OBJS)
$(OBJS): $(ROOT)/include/apue.h
		$(CC) $(CFLAGS) $(INCLS) -c $*.c
clean:
		rm $(EFILE) $(OBJS)
