cmake_minimum_required(VERSION 2.8)

project(crunch)

add_definitions("-Wno-unused-value -Wno-deprecated-writable-strings -Wno-bool-conversion")

add_subdirectory(crnlib)
add_subdirectory(crunch)

