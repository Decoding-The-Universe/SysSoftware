# Define macros
INCLUDE_DIR = /home/dhanush-sai/Desktop/Aryabhatta/MakeDemo5/includes
CFLAGS = -I$(INCLUDE_DIR)
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
	rm -f $(TARGET)

