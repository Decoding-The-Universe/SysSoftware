# Part 2: Makefile with a for loop

# Define a list of directories to clean
DIRS = /home/baswadhanushsai/Desktop/Acad/Aryabhatta/MakeDemo3

# Default rule to build (empty, since this example is for cleanup)
all:

# Clean rule using a for loop
clean:
	@for dir in $(DIRS); do \
	    echo "Cleaning $$dir..."; \
	    rm -f $$dir/*.o; \
	done

