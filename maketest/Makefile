OUTPUT_FILE := hello.out

.PHONY: all clean

all: main.o module.o
	gcc $^ -o $(OUTPUT_FILE)
main.o: main.c module.h
	gcc -I . -c $<
module.o: module.c module.h
	gcc -I . -c $<
clean:
	- rm $(OUTPUT_FILE)
	- rm -fr *.o
	@echo CLEAN DONE
