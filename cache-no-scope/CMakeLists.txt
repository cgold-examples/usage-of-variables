# Top level CMakeLists.txt

cmake_minimum_required(VERSION 2.8)
project(foo NONE)

add_subdirectory(boo)

message("A: ${A}")
