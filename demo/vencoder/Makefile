
CC=arm-linux-gnueabihf-gcc

all:
	$(CC) VideoTest.c \
			-L/usr/local/lib/full-package-name/ \
			-lcedar_vencoder -lcedar_common -lcedar_base\
			-I../../src/base/include/ \
			-I../../src/vencoder/include/ \

clean:
	rm a.out

