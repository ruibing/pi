CC=gcc
CPP=g++
CFLAGS=
CPPFLAGS=
CXXFLAGS=-c -O3 -march=armv6 -mfpu=vfp -mfloat-abi=hard -Wall
LDFLAGS=-lm

all: whetstone

whetstone: whetstone.o
	$(CC) $(LDFLAGS) whetstone.o -o whetstone

whetstone.o: whetstone.c
	$(CC) $(CXXFLAGS) whetstone.c

clean:
	rm -rf *.o whetstone
