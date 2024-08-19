# Define the compiler and flags
CC = gcc
CFLAGS = -Wall -g



# Define macros
INCLUDE = /home/dhanush-sai/Desktop/Aryabhatta/MakeDemo6/includes
CFLAGS5 = -I$(INCLUDE)
LDFLAGS5 = -lm


DRIVER_PATH = /home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/
SHAPES_PATH = /home/dhanush-sai/Desktop/Aryabhatta/MakeDemo3/

# Target executable
EXES = shapes libdriver listprimes

# Default rule	: build all executables
all: $(EXES)



######################4########################################

# Macro for header file paths
INCLUDE_DIRS = -I/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/bar/include -I/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/foo/include

# Macro for library paths
LIB_DIRS = -L/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/foo/lib -L/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/bar/lib

CFLAGS4 = $(INCLUDE_DIRS)
LDFLAGS4 = $(LIB_DIRS)


# Rule to compile libdriver (from Problem 4)
SRCS = /home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/driver.c
TARGET = libdriver
# Libraries to link against
LIBRARIES = -lfoo -lbar

$(TARGET): $(SRCS)
	$(CC) $(CFLAGS4) $(SRCS) -o $(TARGET) $(LDFLAGS4) $(LIBRARIES)



######################3##############################

# Rule to compile shapes (from Problem 3)
shapes: cube.o rectangle.o cylinder.o circle.o sphere.o shape.o
	$(CC) $(CFLAGS) -o $@ $^
	

# Pattern rule to compile .c files into .o files for shapes
%.o: $(SHAPES_PATH)/%.c
	$(CC) $(CFLAGS) -c $< -o $@
	

#####################5################################
# Source files
INCLUDE_DIR5 = /home/dhanush-sai/Desktop/Aryabhatta/MakeDemo6/includes
CFLAGS = -I$(INCLUDE_DIR5)
LDFLAGS = -lm

# Target executable
TARGET = listprimes

# Source files
SRC = main.c listprimes.c linkedlist.c

# Rule to build the executable
$(TARGET): $(SRC)
	$(CC) $(CFLAGS) -o $(TARGET) $(SRC) $(LDFLAGS)


# Clean rule to delete the executable
.PHONY: clean
clean:
	rm -rf *.o shapes
	rm -f $(TARGET) 

