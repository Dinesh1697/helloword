all: hellomake

hellomake: hellomake.o
	cc  hellomake.o -o hellomake

hellomake.o : hellomake.c
	cc -c hellomake.c -o hellomake.o

clean:
	rm -f hellomake

install: all
	mkdir -p ${DESTDIR}${bindir}
	cp -f hellomake ${DESTDIR}${bindir}
	chmod 755 ${DESTDIR}${bindir}/hellomake

.PHONY: all clean install
