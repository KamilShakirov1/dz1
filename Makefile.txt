all:sorts


sorts: sorts.o
	g++ sorts.o -o out

sorts.o: sorts.cpp
	g++ -c sorts.cpp 

clean:
	rm -rf *.o out
