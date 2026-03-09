NAME_STUDENT_1= Caprian_Tudor_A5
NAME_STUDENT_2= X_A5
NAME_HOMEWORK=sg1

CC=gcc
SRC=$(NAME_HOMEWORK).cpp
BINARY=$(NAME_HOMEWORK).bin
CPPFLAGS=-O2 -g0
LDFLAGS=-lGL -lGLU -lglut

EXPORT=$(NAME_STUDENT_1)_$(NAME_STUDENT_2)_$(NAME_HOMEWORK).cpp

all: run

$(BINARY): $(SRC)
	g++ -o $@ $^ $(CPPFLAGS) $(LDFLAGS)

run: $(BINARY)
	./$<

clean:
	rm $(BINARY) *~ $(ARCHIVE) 2>/dev/null || echo -n ''

export: clean
	cp -f $(SRC) $(EXPORT)
