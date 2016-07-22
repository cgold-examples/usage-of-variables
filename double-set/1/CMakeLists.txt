cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(abc "123" CACHE STRING "")
message("Variable from cache: ${abc}")
