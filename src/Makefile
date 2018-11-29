# target
TARGET	= catcpp
# compiler
CXX    	= /usr/local/gcc-4.8.0/bin/g++
LIBS	= -L../libs/ -Wl,-Bdynamic -lrt -lcatclient
CXXFLAGS= -g -std=c++11  -Wall -rdynamic -ldl

CPPFLAGS= -I.  -I../include -I../include/cat -I../include/rabbitmq

SRC	= $(wildcard *.cpp)
OBJ	= $(patsubst %.cpp,%.o,$(SRC) )

# all:$(OBJ) $(TARGET)

$(TARGET):$(OBJ)
	$(CXX) -o $@ $^ $(CXXFLAGS) $(CPPFLAGS) $(LIBS)
clean:
	rm -rf $(TARGET) *.o
