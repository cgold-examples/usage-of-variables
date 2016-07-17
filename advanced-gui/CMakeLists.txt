cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(FOO_A "123" CACHE STRING "")
set(FOO_B "456" CACHE STRING "")
set(FOO_C "789" CACHE STRING "")

mark_as_advanced(FOO_B)
