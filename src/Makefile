OBJS=obj/dig.o obj/display.o obj/files.o obj/hash.o obj/hashlist.o obj/helpers.o obj/main.o obj/multihash.o obj/threadpool.o obj/winpe.o obj/xml.o obj/md5.o obj/sha1.o obj/sha256.o obj/tiger.o obj/whirlpool.o 
ALL_TARGETS=hashdeep md5deep sha1deep sha256deep whirlpooldeep tigerdeep
INSTALL_DIR=/usr/local/bin/
all : $(ALL_TARGETS)
$(ALL_TARGETS) : obj/ $(OBJS)
	g++ -o $@ $(OBJS)

install: all
	cp $(ALL_TARGETS) $(INSTALL_DIR)

obj/: 
	if [ ! -d ./obj ]; then mkdir obj; fi
obj/dig.o : dig.cpp
	g++ -c -o obj/dig.o dig.cpp 
obj/display.o : display.cpp
	g++ -c -o obj/display.o display.cpp 
obj/files.o : files.cpp
	g++ -c -o obj/files.o files.cpp 
obj/hash.o : hash.cpp
	g++ -c -o obj/hash.o hash.cpp 
obj/hashlist.o : hashlist.cpp
	g++ -c -o obj/hashlist.o hashlist.cpp 
obj/helpers.o : helpers.cpp
	g++ -c -o obj/helpers.o helpers.cpp 
obj/main.o : main.cpp
	g++ -c -o obj/main.o main.cpp 
obj/multihash.o : multihash.cpp
	g++ -c -o obj/multihash.o multihash.cpp 
obj/threadpool.o : threadpool.cpp
	g++ -c -o obj/threadpool.o threadpool.cpp 
obj/winpe.o : winpe.cpp
	g++ -c -o obj/winpe.o winpe.cpp 
obj/xml.o : xml.cpp
	g++ -c -o obj/xml.o xml.cpp 
obj/md5.o : md5.c
	gcc -c -o obj/md5.o md5.c
obj/sha1.o : sha1.c
	gcc -c -o obj/sha1.o sha1.c
obj/sha256.o : sha256.c
	gcc -c -o obj/sha256.o sha256.c
obj/tiger.o : tiger.c
	gcc -c -o obj/tiger.o tiger.c
obj/whirlpool.o : whirlpool.c
	gcc -c -o obj/whirlpool.o whirlpool.c
