cc = gcc
CFLAGS = -Wall -Iinclude

SRC = src/*.c # main.c add.c 로 해도 됨
OBJ = $(SRC:.c=.o) # src/main.o src/add.o
# 디버깅 할 때 echo로 하면 됨

.PHONY: all clean

app: $(OBJ)
	$(cc) $(CFLAGS) $^ -o $@

%.o: %.c %.h
	$(cc) $(CFLAGS) -c $< 

clean:
	rm -rf app *.o

helloTest: abc def
	echo $@
abc:
	@echo abc
# @ 빼면 echo abc도 출력되고, abc도 출력됨.
def:
	@echo def