# Define the compiler and flags
CC = gcc
CFLAGS = -Wall -g

# Macro for the header file path
INCLUDE = -I./include

# Define the executable name
EXEC = listprimes

# Default rule: build the executable
all: $(EXEC)

# Rule to compile listprimes.c into an executable
$(EXEC): listprimes.c
	$(CC) $(CFLAGS) $(INCLUDE) -o $@ $<

# Clean rule to remove the executable
clean:
	rm -f $(EXEC)

