cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(A "123" CACHE STRING "" FORCE)
message("A: ${A}")
