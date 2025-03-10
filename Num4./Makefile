clear:
	rm -rf *.o *.a *_test


# ---

add.o: add.c add.h
	gcc -g -c add.c -o add.o

add.a: add.o
	ar rc add.a add.o

add_test.o: add_test.c add.h
	gcc -g -c add_test.c -o add_test.o

add_test: add_test.o add.a
	gcc -g -o add_test add_test.o add.a 


test: add_test
	./add_test