cc = gcc
CFLAGS = -Wall

OBJ = main.o add.o

.PHONY: all clean

app: $(OBJ)
	$(cc) $(CFLAGS) $^ -o $@

%.o: %.c %.h
	$(cc) $(CFLAGS) -c $< -o $@

clean:
	rm -rf app *.o

helloTest: abc def
	echo $^
abc:
	@echo abc
# @ 빼면 echo abc도 출력되고, abc도 출력됨.
def:
	@echo def