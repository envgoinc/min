cmake_minimum_required(VERSION 3.6)
project(min)
set(CMAKE_VERBOSE_MAKEFILE ON)
set(CMAKE_C_STANDARD 90)

set(SOURCE_FILES
        src/min.c
        src/min.h)

add_compile_options(
        -Wall
        -Wextra
        # -Wpedantic
)

add_library(min STATIC ${SOURCE_FILES})
# target_compile_options(min PUBLIC -nostdlib -mcpu=cortex-m0plus -mtune=cortex-m0plus -mthumb -g -O3 -Wall)

target_include_directories(min PUBLIC ${PROJECT_SOURCE_DIR})
