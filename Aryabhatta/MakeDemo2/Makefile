# Makefile for compiling shapes executable

# Define the compiler
CC = gcc

# Define the flags to pass to the compiler
CFLAGS = -Wall -g

# Define the object files
OBJS = cube.o rectangle.o cylinder.o circle.o sphere.o shape.o

# Define the executable name
EXEC = shapes

# Rule to link the object files and create the executable
$(EXEC): $(OBJS)
	$(CC) $(CFLAGS) -o $(EXEC) $(OBJS)

# Rules to compile each .c file into .o file
cube.o: cube.c
	$(CC) $(CFLAGS) -c cube.c

rectangle.o: rectangle.c
	$(CC) $(CFLAGS) -c rectangle.c

cylinder.o: cylinder.c
	$(CC) $(CFLAGS) -c cylinder.c

circle.o: circle.c
	$(CC) $(CFLAGS) -c circle.c
	
sphere.o: sphere.c
	$(CC) $(CFLAGS) -c sphere.c
	
shape.o: shape.c
	$(CC) $(CFLAGS) -c shape.c

# Clean rule to remove the compiled files
clean:
	rm -f $(OBJS) $(EXEC)





# all:
#	gcc -c *.c 
#	gcc -o shape *.o
#clean:
#	rm -f *.o shape

