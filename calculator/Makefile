SOURCES = $(wildcard *.c)
OBJECTS = $(SOURCES:.c=.o)
EXECUTABLE = calculator

# Compile .c into .o
%.o: %.c
	gcc -c $< -o $@

# Link .o files to executable calculator
$(EXECUTABLE): $(OBJECTS)
	gcc $^ -g -o $@

# Delete all .o files
clean:
	rm -f $(OBJECTS)

.PHONY: clean
