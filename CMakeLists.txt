cmake_minimum_required(VERSION 3.1)
message("Building periphery")
project(periphery C)

file(GLOB_RECURSE ${PROJECT_NAME}_SOURCES src/*.c)

add_library(${PROJECT_NAME} INTERFACE)
target_include_directories(${PROJECT_NAME} INTERFACE src)
