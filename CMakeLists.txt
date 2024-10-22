# Minimum CMake version
cmake_minimum_required(VERSION 3.10)

# Project name
project(one)

# Specify the C++ standard
set(CMAKE_CXX_STANDARD 14)

# Add the source files for the library
add_library(one STATIC src/libone.cpp)

# Specify the include directories
target_include_directories(one PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}/src)
