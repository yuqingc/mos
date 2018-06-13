all: main.o module.o
	gcc main.o module.o -o hello.out
main.o: main.c module.h
	gcc -I . -c main.c
module.o: module.c module.h
	gcc -I . -c module.c
clean:
	rm -fr *.o
	rm hello

.PHONY: all clean
