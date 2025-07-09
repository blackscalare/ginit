
CC = gcc
CFLAGS = -Wall -std=c99 -I/usr/local/include -Isrc

SRC_DIR = src
OBJ_DIR = build

SOURCES := $(wildcard $(SRC_DIR)/*.c)
OBJECTS := $(patsubst $(SRC_DIR)/%.c,$(OBJ_DIR)/%.o,$(SOURCES))

TARGET = PROJECT_NAME

$(OBJ_DIR)/%.o: $(SRC_DIR)/%.c
	@mkdir -p $(OBJ_DIR)
	$(CC) $(CFLAGS) -c $< -o $@

$(TARGET): $(OBJECTS)
	$(CC) $(OBJECTS) -o $@ $(LDFLAGS)

all: $(TARGET)

clean:
	rm -rf $(OBJ_DIR) $(TARGET)
