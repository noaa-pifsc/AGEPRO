# Makefile to build agepro.exe from C sources with headers in include/

# Compiler and flags
CC = gcc
CFLAGS = -Iinclude -Wall -O2

# Source and object files
SRCS = agepro.c boxmuller.c ranx.c util.c
OBJS = boxmuller.o ranx.o util.o

# Target executable
TARGET = agepro.exe

# Default target
all: $(TARGET)

# Link executable
$(TARGET): agepro.o $(OBJS)
	$(CC) $(CFLAGS) -o $@ $^ -lm

# Compile .c files to .o files
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Clean up build artifacts
clean:
	rm -f *.o $(TARGET)
