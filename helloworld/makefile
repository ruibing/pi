CC=cc
CFLAGS=-c -Wall

all: helloworld

helloworld: main.o
	$(CC) main.o -o helloworld

main.o: main.c
	$(CC) $(CFLAGS) main.c

clean:
	rm -rf *.o helloworld
