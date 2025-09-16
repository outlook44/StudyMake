# Makefile для example-3333
.PHONY: all debug release clean

# Объявление переменных
CXX = g++                            # Компилятор C++
RELEASE_FLAGS = -O2 -Wall -DNDEBUG  # Флаги для релизной сборки
DEBUG_FLAGS = -g -O0 -Wall          # Флаги для отладочной сборки
RELEASE_EXEC = Kazino-Royal         # Имя релизного исполняемого файла
DEBUG_EXEC = Kazino-Royal-dbg       # Имя отладочного исполняемого файла
SOURCE = Kazino-Royal.cpp           # Имя исходного файла

# Цели
all: debug release

# Правило для отладочной сборки
$(DEBUG_EXEC): $(SOURCE)
	$(CXX) $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC)

debug: $(DEBUG_EXEC)

# Правило для релизной сборки
$(RELEASE_EXEC): $(SOURCE)
	$(CXX) $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

release: $(RELEASE_EXEC)

# Очистка
clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC) *.o



