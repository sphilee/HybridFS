Project : bbfs.o log.o
	gcc -o bbfs bbfs.o log.o -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26 -lfuse

bbfs.o : bbfs.c log.h
	gcc -c bbfs.c -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26 -lfuse

log.o : log.c log.h
	gcc -c log.c -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26 -lfuse

clean :
	rm *.o bbfs
