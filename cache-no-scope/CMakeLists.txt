# Top level CMakeLists.txt

cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

add_subdirectory(boo)

message("A: ${A}")
