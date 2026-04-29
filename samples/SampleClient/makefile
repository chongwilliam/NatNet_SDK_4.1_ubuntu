include=-I../../include
libpath=-L../../lib
libs=-lNatNet
CXXFLAGS = -std=c++17 -I/usr/include/eigen3/ -I/usr/include/jsoncpp -I/usr/include/hiredis

all:build/SampleClient

build/SampleClient: 
	g++ SampleClient.cpp $(include) $(libpath) $(libs) ${CXXFLAGS} -ljsoncpp -lpthread -lhiredis -o build/SampleClient

.PHONY: clean
clean:
	@rm -f ./build/SampleClient
