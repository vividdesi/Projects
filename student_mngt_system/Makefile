# Compiler
CC = gcc

# Compiler flags
CFLAGS = -Wall -Iinclude
DEBUGFLAGS = -g -O0 -Wall -Iinclude

# Source files
SRCS = src/main.c src/functions.c src/insert.c src/delete.c

# Object files
OBJS = main.o functions.o insert.o delete.o

# Target executable
TARGET = program
DEBUG_TARGET = Debug_project

# Default target
all: $(TARGET)

# Compile object files
main.o: src/main.c include/header.h
	$(CC) $(CFLAGS) -c src/main.c -o main.o

functions.o: src/functions.c include/header.h
	$(CC) $(CFLAGS) -c src/functions.c -o functions.o

insert.o: src/insert.c include/header.h
	$(CC) $(CFLAGS) -c src/insert.c -o insert.o

delete.o: src/delete.c include/header.h
	$(CC) $(CFLAGS) -c src/delete.c -o delete.o

# Link object files to create executable
$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) $(OBJS) -o $(TARGET)

# Debug target (compile all source files directly with debug flags)
Debug: 
	$(CC) $(DEBUGFLAGS) $(SRCS) -o $(DEBUG_TARGET)

# Clean object files and executables
clean:
	rm -f *.o $(TARGET) $(DEBUG_TARGET)

.PHONY: all Debug clean

