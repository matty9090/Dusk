cmake_minimum_required(VERSION 3.5)
project(dusk)

set(CMAKE_CXX_STANDARD 14)

include_directories(Source)

file(GLOB_RECURSE SRC_FILES Source/*.cpp)
message(${SRC_FILES})

add_library(nbody ${SRC_FILES})