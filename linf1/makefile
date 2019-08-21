#LInk do tutorial 
#http://www.cs.colby.edu/maxwell/courses/tutorials/maketutor/


# make1

# hellomake: hellomake.cpp hellofunc.cpp
# 		g++ -c hellofunc.cpp 
# 		g++ -o main hellomake.cpp hellofunc.o
# 		./main

# # make 2
# CC = g++
# CFLAGS = -I.

# hellomake: hellomake.cpp hellofunc.cpp
# 		$(CC)-c hellofunc.cpp 
# 		$(CC) -o main hellomake.cpp hellofunc.o
# 		./main

#make 3

CC=g++
CFLAGS=-I.
DEPS=hellomake.hpp

%.o : %.cpp $(DEPS)
		$(CC) -c $@ $< 
hellomake: hellofunc.o
		$(CC) -o hellomake hellomake.cpp hellofunc.o 
		./main



	# #makefile para o trabalho

	# IDIR =../include
	# CC=gcc
	# CFLAGS=-I$(IDIR)

	# ODIR=obj
	# LDIR =../lib

	# LIBS=-lm

	# _DEPS = hellomake.h
	# DEPS = $(patsubst %,$(IDIR)/%,$(_DEPS))

	# _OBJ = hellomake.o hellofunc.o 
	# OBJ = $(patsubst %,$(ODIR)/%,$(_OBJ))


	# $(ODIR)/%.o: %.c $(DEPS)
	# 	$(CC) -c -o $@ $< $(CFLAGS)

	# hellomake: $(OBJ)
	# 	$(CC) -o $@ $^ $(CFLAGS) $(LIBS)

	# .PHONY: clean

	# clean:
	# 	rm -f $(ODIR)/*.o *~ core $(INCDIR)/*~ 