# Makefile для example-3 (C++ версия)

.PHONY: all debug release clean

# Компилятор C++ и флаги
CXX = g++
RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall

# Имена файлов
SOURCE = Kazino-Royal.cpp
RELEASE_EXEC = program
DEBUG_EXEC = program-dbg

all: debug release

debug: $(DEBUG_EXEC)

release: $(RELEASE_EXEC)

# Сборка release версии
$(RELEASE_EXEC): $(SOURCE)
	$(CXX) $(RELEASE_FLAGS) $(SOURCE) -o $(RELEASE_EXEC)

# Сборка debug версии
$(DEBUG_EXEC): $(SOURCE)
	$(CXX) $(DEBUG_FLAGS) $(SOURCE) -o $(DEBUG_EXEC)

clean:
	rm -f $(RELEASE_EXEC) $(DEBUG_EXEC) *.o