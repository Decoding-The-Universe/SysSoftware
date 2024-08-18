# Macro for header file paths
INCLUDE_DIRS = -I/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/bar/include -I/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/foo/include

# Macro for library paths
LIB_DIRS = -L/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/foo/lib -L/home/dhanush-sai/Desktop/Aryabhatta/MakeDemo4/bar/lib

# Compiler and flags
CC = gcc
CFLAGS = $(INCLUDE_DIRS)
LDFLAGS = $(LIB_DIRS)

# Libraries to link against
LIBRARIES = -lfoo -lbar

# Source files and target executable
SRCS = driver.c
TARGET = libdriver

# Default rule to build the executable
$(TARGET): $(SRCS)
	$(CC) $(CFLAGS) $(SRCS) -o $(TARGET) $(LDFLAGS) $(LIBRARIES)

# Clean rule to delete the executable
clean:
	rm -f $(TARGET) a.out
