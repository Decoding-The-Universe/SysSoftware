# Define the compiler and the include path
CXX = g++
CXXFLAGS = -I/usr/include/GL

# Name of the executable
TARGET = intertrbobarm

# Source file
SRC = intertrbobarm.cpp

# Rule to build the executable
all: $(TARGET)

$(TARGET): $(SRC)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(SRC) -lGL -lGLU -lglut

# Clean rule to remove the executable
clean:
	rm -f $(TARGET)

