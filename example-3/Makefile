.PHONY: all clean

# Флаги компиляции
RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall

# Имена исполняемых файлов
RELEASE_EXEC = kazino
DEBUG_EXEC   = kazino-dbg

# Исходный файл
SOURCE = Kazino-Royal.cpp

# Цели
all: debug release

debug: $(DEBUG_EXEC)

$(DEBUG_EXEC): $(SOURCE)
	g++ $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC)

release: $(RELEASE_EXEC)

$(RELEASE_EXEC): $(SOURCE)
	g++ $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC)


