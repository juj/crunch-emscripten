cmake_minimum_required(VERSION 2.8)

file(GLOB sourceFiles *.*)

include_directories(../crnlib)
include_directories(../inc)

add_executable(crunch ${sourceFiles})

target_link_libraries(crunch crnlib)