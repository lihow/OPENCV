CC = g++

CFLAGS += -g -O3 -Wall
INC += -I. `pkg-config --cflags opencv`
LIBS += `pkg-config --libs opencv`

TARGET = main.bin
OBJS += main.o \


#all:$(TARGET)
#$(TARGET):$(OBJS)
#	$(CC) $(INC) $(CFLAGS) $(OBJS) -o $(TARGET) $(LIBS)
#$(OBJS):%.o:%.cpp
#	$(CC) $(INC) $(CFLAGS) -c $< -o $@

$(TARGET):main.cpp
	$(CC) $(INC) $(CFLASS)  main.cpp -o $@ $(LIBS)

.PHONY:clean
clean:
	rm -r  $(TARGET)
