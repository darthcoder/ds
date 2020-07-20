cmake_minimum_required(VERSION 3.17)
project(ds C)

set(CMAKE_C_STANDARD 11)
set(SOURCE_FILES main.c)
set(CMAKE_C_FLAGS "-I/usr/local/include/SDL2 -D_THREAD_SAFE -L/usr/local/lib -lSDL2" )
add_executable(ds main.c function.c function.h)