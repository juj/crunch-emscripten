cmake_minimum_required(VERSION 2.8)

file(GLOB sourceFiles crn_*.*)
file(GLOB lzmaFiles lzma_*.*)

message(STATUS ${sourceFiles} ${lzmaFiles} crnlib.cpp)

include_directories(../inc)

add_library(crnlib STATIC ${sourceFiles} ${lzmaFiles} crnlib.cpp)
