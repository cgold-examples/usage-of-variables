cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(a "123")
set(a "789" CACHE STRING "")

message("Regular variable unset, take from cache: ${a}")
