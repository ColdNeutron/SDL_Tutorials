
CC = clang

INCLUDE_PATHS = -IC:\devlib\mingw\x64\include\SDL2
LIBRARY_PATHS = -LC:\devlib\mingw\x64\lib

# -w suppresses all warnings
# -Wl,-subsystem,windows gets rid of the console window
COMPILER_FLAGS = -w -Wl,-subsystem,windows
LINKER_FLAGS = -lmingw32 -lSDL2main -lSDL2

OBJS = 04_key_presses.c
OBJ_NAME = 04.exe


all: $(OBJS)
	$(CC) $(OBJS) $(INCLUDE_PATHS) $(LIBRARY_PATHS) $(COMPILER_FLAGS) $(LINKER_FLAGS) -o $(OBJ_NAME)

run: $(OBJS)
	.\$(OBJ_NAME)

clean:
	del .\$(OBJ_NAME)