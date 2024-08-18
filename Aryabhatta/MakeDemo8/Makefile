#install gl if it is not installed in your system by $sudo apt-get install libglu1-mesa-dev freeglut3-dev mesa-common-dev
# many other GL examples are at https://cs.lmu.edu/~ray/notes/openglexamples/
#
#CC =gcc CCFLAG=-fno-threadsafe-statics LDFLAG= -lGL -lglut -lGLU -lm SRC=intertrbobarm

all:

	gcc  -fno-threadsafe-statics -o intertrbobarm intertrbobarm.cpp -lGL -lglut -lGLU -lm
clean:
	rm -rf *.o *.exe

.PHONY: all clean

