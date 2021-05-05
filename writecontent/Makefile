CFLAGS=-g -I. -Wall -O2   

all: writeeepromcontent 

clean: 
	rm -f writeeepromcontent writeeepromcontent.o

eeprog: writeeepromcontent.o 

eeprog-static: writeeepromcontent.o 
	$(CC) -static -o $@ $?

.PHONY: install
install: writeeepromcontent
	install writeeepromcontent /usr/local/bin