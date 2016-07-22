cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(FOO_A "123" CACHE INTERNAL "")
set(FOO_A "456" CACHE INTERNAL "")
set(FOO_A "789" CACHE INTERNAL "")

set(FOO_B "123" CACHE STRING "")
set(FOO_B "456" CACHE STRING "")
set(FOO_B "789" CACHE STRING "")

message("FOO_A (internal): ${FOO_A}")
message("FOO_B (string): ${FOO_B}")
