# Variables
CC = gcc
CFLAGS = -I./submodule -Wall
OBJ = main.o submodule/src/submodule.o
TARGET = main

# Default target
all: $(TARGET)

# Link objects to create the final executable
$(TARGET): $(OBJ)
	$(CC) -o $(TARGET) $(OBJ)

# Compile main.c to main.o
main.o: main.c
	$(CC) $(CFLAGS) -c main.c

# Compile submodule.c to submodule.o
submodule/submodule.o: submodule/src/submodule.c
	$(CC) $(CFLAGS) -c submodule/src/submodule.c -o submodule/src/submodule.o

# Clean up build files
clean:
	rm -f $(OBJ) $(TARGET)

# PHONY targets to avoid conflicts with files named "all" or "clean"
.PHONY: all clean
