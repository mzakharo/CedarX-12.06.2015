CC=arm-linux-gnueabihf-gcc

CFLAGS := -O2 -g -Wall

LIBCEDAR='cedarx'
PKGCONFIG := $(shell pkg-config --help 2> /dev/null)
ifndef PKGCONFIG
    $(error "pkg-config is not available please install pkg-config")
endif
CFLAGS += $(shell pkg-config --cflags $(LIBCEDAR))
LDFLAGS += $(shell pkg-config --libs $(LIBCEDAR))

all: venc

venc: VideoTest.c
	$(CC) $< $(CFLAGS) $(LDFLAGS) -o $@

clean:
	rm -rf venc

