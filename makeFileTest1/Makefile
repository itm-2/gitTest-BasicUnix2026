SRC = $(wildcard *.c) # src/main.c src/add.c
OBJ = $(patsubst %.c, %.o, $(SRC)) # main.o add.o, src에 있는 모든 .c 파일을 .o 파일로 변환
echo: $(SRC) # src/main.c src/add.c
	@echo $^ 
	@echo $<
	@echo $@
	@echo $(OBJ)
	@echo $(patsubst %.c, %.o, $(SRC)) 