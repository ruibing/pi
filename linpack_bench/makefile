CC=gcc
CPP=g++
CFLAGS=
CPPFLAGS=
CXXFLAGS=-c -O3 -march=armv6 -mfpu=vfp -mfloat-abi=hard -Wall
LDFLAGS=-lm

all: linpack_bench linpack_bench_d linpack_bench_s

linpack_bench: linpack_bench.o
	$(CC) $(LDFLAGS) linpack_bench.o -o linpack_bench

linpack_bench_d: linpack_bench_d.o
	$(CPP) $(LDFLAGS) linpack_bench_d.o -o linpack_bench_d

linpack_bench_s: linpack_bench_s.o
	$(CPP) $(LDFLAGS) linpack_bench_s.o -o linpack_bench_s

linpack_bench.o: linpack_bench.c
	$(CC) $(CXXFLAGS) linpack_bench.c

linpack_bench_d.o: linpack_bench_d.cpp
	$(CPP) $(CXXFLAGS) linpack_bench_d.cpp

linpack_bench_s.o: linpack_bench_s.cpp
	$(CPP) $(CXXFLAGS) linpack_bench_s.cpp

clean:
	rm -rf *.o linpack_bench linpack_bench_d linpack_bench_s
