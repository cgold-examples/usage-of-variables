cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(FOO_A "Default value for A" CACHE STRING "")
set(FOO_B "Default value for B")

message("FOO_A: ${FOO_A}")
message("FOO_B: ${FOO_B}")
