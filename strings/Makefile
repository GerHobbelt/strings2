EXE=strings2

CC=g++
CFLAGS=-Wall -std=c++17
LD=$(CC)
LDFLAGS=
LIBS=
SRC=strings.cpp string_parser.cpp binary2strings.cpp print_buffer.cpp extracted_string.cpp
OBJ=$(SRC:.cpp=.o)

.PHONY: all clean

all: $(EXE)

$(EXE): $(OBJ)
	$(LD) $(LDFLAGS) -o $@ $^ $(LIBS)

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ) $(EXE)
