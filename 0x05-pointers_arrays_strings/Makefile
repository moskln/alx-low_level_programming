CC = gcc
CFLAGS = -Wall -Wextra -Werror -pedantic

SRC = 2-main.c 2-strlen.c
OBJ = $(SRC:.c=.o)
TARGET = 2-main

all: $(TARGET)

$(TARGET): $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) -o $(TARGET)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(TARGET)

re: fclean all

.PHONY: all clean fclean re

