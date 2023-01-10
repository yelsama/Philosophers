NAME = philo

SOURCES = main.c philos_life.c main_utils.c philos_life_utils.c philos_lucked_funcs.c \

OBJECTS = $(SOURCES:%.c=%.o)

CC = cc
CFLAGS = -Wall -Wextra -Werror -pthread -g

all: $(NAME)

$(NAME):$(OBJECTS)
	$(CC) $(CFLAGS) -o $(NAME) $(OBJECTS)

run: all
	./$(NAME) $$ARG

st: 
	make run ARG="200 450 200 200 40"

mt: 
	make run ARG="3 200 100 300 2"

lt: 
	make run ARG="9 3 3 3"

clean:
	/bin/rm -f $(OBJECTS)

fclean: clean
	/bin/rm -f $(NAME)

re: fclean all