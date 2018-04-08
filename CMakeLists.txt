cmake_minimum_required(VERSION 3.1)
message("Building periphery")
project(periphery)

file(GLOB_RECURSE ${PROJECT_NAME}_SOURCES src/*.c)

add_library(${PROJECT_NAME} STATIC ${${PROJECT_NAME}_SOURCES})
target_include_directories(${PROJECT_NAME} INTERFACE src)
