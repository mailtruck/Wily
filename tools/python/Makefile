# 9term
CC=gcc
PYTHONINC=/n/staff/srce/usr/local/bin/python/Python-1.4/Include/
CFLAGS=-g -Wall -I. -I/usr/pgrad/gary/src/wily/include -I/usr/pgrad/gary/src/wily/sam/include -I$(PYTHONINC) -DNDEBUG

XLIBS=-L/usr/pgrad/gary/obj/sun4d/wily/libmsg -l msg -lsocket -lnsl -lintl

target: wilymodule.so
OBJS=wilymodule.o

wilymodule.so:	$(OBJS) Makefile /usr/pgrad/gary/obj/sun4d/wily/libmsg/libmsg.a
	ld -G -o wilymodule.so wilymodule.o $(XLIBS)

wilymodule.o:	/usr/pgrad/gary/src/wily/include/msg.h
