cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(FOO_A "123" CACHE STRING "")
set(FOO_B "456" CACHE INTERNAL "")
set(FOO_C "789" CACHE STRING "")
