NAME = libft.a
SOURCES = ft_atoi.c ft_isdigit.c ft_isspace.c \
	ft_strlen.c ft_putchar_fd.c ft_putstr_fd.c ft_putnbr_fd.c

OBJECTS = $(SOURCES:.c=.o)

CC = gcc
CFLAGS = -Wall -Wextra -Werror

all: $(NAME)

$(NAME): $(OBJECTS)
	$(AR) -r $@ $?

%.o: %.c
	$(CC) -c $(CFLAGS) $?

clean:
	rm -f $(OBJECTS) $(BOBJECTS)

fclean: clean
	rm -f $(NAME)

re: fclean all

.PHONY: all bonus clean fclean re
