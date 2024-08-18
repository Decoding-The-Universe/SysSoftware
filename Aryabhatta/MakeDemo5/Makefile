CC = gcc 
CFLAGS = -I./include -Wall
SRCS = main.c linkedlist.c listprimes.c
OBJS = $(SRCS:.c=.o)
EXEC = program 

all : $(EXEC)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

$(EXEC): $(OBJS)
	$(CC) $(CFLAGS) -o $@ $(OBJS) -lm

clean : 
	rm -f $(OBJS) $(EXEC)
