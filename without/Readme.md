g++ -c hello.cpp -o hello.o
ar rcs libhello.a 
g++ -Wall -Wextra -O2 main.cpp -o main.elf -L. -lhello
