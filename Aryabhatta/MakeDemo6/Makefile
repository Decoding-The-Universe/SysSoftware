# Makefile for combining multiple Makefiles into one

# Define the compiler and flags
CC = gcc
CFLAGS = -Wall -g

# Macro for the library paths and header files (from Problem 3 and Problem 5)
LIBS = -I/home/baswadhanushsai/Desktop/Acad/Aryabhatta/dependinces -L/home/baswadhanushsai/Desktop/Acad/Aryabhatta/dependinces -lfoo -lbar

# Macro for the header file path (from Problem 5)
INCLUDE = -I./include

# Macro for the path to driver.c
# Replace /path/to/driver/ with the actual path to the directory containing driver.c
DRIVER_PATH = /home/baswadhanushsai/Desktop/Acad/Aryabhatta/MakeDemo4
SHAPES_PATH = /home/baswadhanushsai/Desktop/Acad/Aryabhatta/MakeDemo3

# Macro for the executables
EXES = shapes libdriver listprimes
	
# Default rule	: build all executables
all: $(EXES)

# Rule to compile shapes (from Problem 3)
shapes: cube.o rectangle.o cylinder.o circle.o sphere.o
	$(CC) $(CFLAGS) -o $@ $^

# Rule to compile libdriver (from Problem 4)
libdriver: $(DRIVER_PATH)/driver.c
	$(CC) $(CFLAGS) $(LIBS) -o $@ $<

# Rule to compile listprimes (from Problem 5)
listprimes: listprimes.c
	$(CC) $(CFLAGS) $(INCLUDE) -o $@ $<

# Pattern rule to compile .c files into .o files for shapes
%.o: $(SHAPES_PATH)/%.c
	$(CC) $(CFLAGS) -c $< -o $@

# Clean rule to remove all object files and executables
clean:
	rm -f *.o $(EXES)

