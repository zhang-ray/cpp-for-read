cmake_minimum_required(VERSION 3.0.0)

set(PROJECT_NAME cpp-for-read)
set(CMAKE_CXX_STANDARD 14)

project(${PROJECT_NAME})

include_directories(.)
file(GLOB_RECURSE FILES_SOURCES *.cpp *.cc *.c)
file(GLOB_RECURSE FILES_INCLUDE *.hpp *.hh *.h)

add_library(${PROJECT_NAME} STATIC ${FILES_INCLUDE} ${FILES_SOURCES})
