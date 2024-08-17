# Target executable
TARGET = main

# Source files
SOURCES = main.c

# Default rule to build the executable
all: $(TARGET)

# Rule to compile the executable
$(TARGET): $(SOURCES)
	@echo "Compiling $(SOURCES) into $(TARGET)..."
	gcc $(SOURCES) -o $(TARGET)

# Clean rule to delete the executable
clean:
	@echo "Cleaning up..."
	rm -f $(TARGET)

# Ensure make doesn't delete intermediate files
.PHONY: all clean

