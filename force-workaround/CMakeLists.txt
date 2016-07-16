cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(A "123")
set(A "456" CACHE STRING "" FORCE)

message("A: ${A}")
