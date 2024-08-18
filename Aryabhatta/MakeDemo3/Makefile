# Define the compiler and flags
CC = gcc
CFLAGS = -Wall -g
RED := \033[31m

# Define the source files and the corresponding object files
SRCS = cube.c rectangle.c cylinder.c circle.c sphere.c shape.c
OBJS = $(SRCS:.c=.o)
MESSAGE := "Hello, World!"

# Define the executable name
EXEC = shapes

# Default rule: build the executable
all: $(EXEC)
	@echo "$(RED) $(MESSAGE) $(RESET)"
	
# Rule to link all object files into the executable
$(EXEC): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^

# Pattern rule to compile .c files into .o files
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Clean rule to remove all object files and the executable
clean:
	rm -f $(OBJS) $(EXEC)

