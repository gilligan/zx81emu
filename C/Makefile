all: zx81

zx81: zx81.o simz80.o
	gcc -o zx81 zx81.o simz80.o -framework OpenGL -framework Cocoa  -lSDL -lSDLmain

zx81.o: zx81.c zx81rom.h
	gcc -O3 -c zx81.c

simz80.o: simz80.c simz80.h
	gcc -O3 -c simz80.c

clean:
	rm -f zx81.exe zx81.o simz80.o
