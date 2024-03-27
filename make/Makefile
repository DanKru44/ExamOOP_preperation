all : main.elf

main.elf: libhello.a
	g++ -Wall -Wextra -O2 main.cpp -o main.elf -L. -lhello

libhello.a: hello.o
	ar rcs libhello.a hello.o

hello.o:
	g++ -c hello.cpp -o hello.o

clean:
	rm -r main.elf hello.o libhello.a

.PHONY: all clean
