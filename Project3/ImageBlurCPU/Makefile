CC = g++
CFLAGS = -std=c++11 -Wall -g

SRCS = ./src/ImageBlurCPU.cpp
OBJS = $(SRCS:.cpp=.o)
EXEC = ImageBlurCPU

all: $(EXEC)

$(EXEC): $(OBJS)
	$(CC) $(CFLAGS) $(OBJS) -o $(EXEC)

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJS) $(EXEC)
