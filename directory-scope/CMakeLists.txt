# Top level CMakeLists.txt

cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(abc "123")

message("Top level scope (before): ${abc}")

add_subdirectory(boo)

message("Top level scope (after): ${abc}")
