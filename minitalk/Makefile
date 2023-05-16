SERVER = server

CLIENT = client

CLIENT_BONUS = client_bonus

SERVER_BONUS = server_bonus

CC = gcc

CFLAGS = -Wall -Werror -Wextra

SOURCE = minitalk_utils.c

OBJ = $(SOURCE:.c=.o)

DEFS = minitalk.h

# Colors

DEF_COLOR = \033[0;39m
GRAY = \033[0;90m
RED = \033[0;91m
GREEN = \033[0;92m
YELLOW = \033[0;93m
BLUE = \033[0;94m
MAGENTA = \033[0;95m
CYAN = \033[0;96m
WHITE = \033[0;97m

all: $(SERVER) $(CLIENT)

$(SERVER) : server.c $(DEFS)
	$(CC) $(CFLAGS) server.c $(SOURCE) -o server
$(CLIENT) : client.c $(DEFS)
	$(CC) $(CFLAGS) client.c $(SOURCE) -o client
	@echo "$(GREEN)Client and Server created!! $(RED) Eurekaa!$(DEF_COLOR)"
	
bonus: $(SERVER_BONUS) $(CLIENT_BONUS)

$(SERVER_BONUS) : server_bonus.c $(DEFS)
	$(CC) $(CFLAGS) server_bonus.c $(SOURCE) -o server_bonus
$(CLIENT_BONUS) : client_bonus.c $(DEFS)
	$(CC) $(CFLAGS) client_bonus.c $(SOURCE) -o client_bonus

clean: 
	@rm -rf $(OBJ)

fclean: clean
	@rm -rf $(SERVER) $(CLIENT) $(SERVER_BONUS) $(CLIENT_BONUS)
	@echo "$(GREEN)Client and Server erased!!$(RED)!!!!$(DEF_COLOR)"

re: fclean all
