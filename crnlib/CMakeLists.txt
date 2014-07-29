cmake_minimum_required(VERSION 2.8)

file(GLOB sourceFiles crn_*.cpp)
file(GLOB lzmaFiles lzma_*.cpp)

message(STATUS ${sourceFiles} ${lzmaFiles} crnlib.cpp)

include_directories(../inc)

add_library(crnlib STATIC ${sourceFiles} ${lzmaFiles} crnlib.cpp)
