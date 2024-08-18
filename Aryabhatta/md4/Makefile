# Define the compiler and flags
CC = gcc
CFLAGS = -Wall -g

# Macro for library and header file paths
LIBS = -I/home/baswadhanushsai/Desktop/Acad/Aryabhatta/dependinces -L/home/baswadhanushsai/Desktop/Acad/Aryabhatta/dependinces -lfoo -lbar

# Define the executable name
EXEC = libdriver

# Default rule: build the executable
all: $(EXEC)

# Rule to compile driver.c and link with the specified libraries
$(EXEC): driver.c
	$(CC) $(CFLAGS) -o $@ $< $(LIBS)

# Clean rule to remove the executable
clean:
	rm -f $(EXEC)

