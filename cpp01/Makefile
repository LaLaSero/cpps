NAME = megaphone
SRCS = srcs/main.c srcs/check_args.c srcs/utils_func.c srcs/life_of_philo.c srcs/process_game.c 
INCLUDE = includes
CC = gcc
CFLAGS = -Wall -Wextra -Werror -std=c++98
OBJS = $(SRCS:.c=.o)

all: $(NAME)

$(NAME): $(OBJS)
	$(CC) $(CFLAGS) -o $(NAME) $(OBJS)

%.o: %.c $(INCLUDE)
	$(CC) -c $(CFLAGS) -o $@ $< -I $(INCLUDE)

clean:
	rm -f $(OBJS)

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all clean fclean re
