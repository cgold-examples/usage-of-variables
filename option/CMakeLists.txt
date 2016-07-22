cmake_minimum_required(VERSION 2.8)
project(foo NONE)

option(FOO_A "Option A" OFF)
option(FOO_B "Option A" ON)

message("FOO_A: ${FOO_A}")
message("FOO_B: ${FOO_B}")
