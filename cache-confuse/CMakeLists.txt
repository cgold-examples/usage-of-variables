cmake_minimum_required(VERSION 2.8)
project(foo NONE)

function(set_abc_globally)
  message("Function scope before cache modify = ${abc}")
  set(abc "789" CACHE STRING "")
  message("Function scope after cache modify = ${abc}")
endfunction()

set(abc "123")

set_abc_globally()

message("Parent scope is not affected, take variable from current scope, not cache = ${abc}")
