cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(X "123" CACHE STRING "X variable")
set(X "456")
message("[0] X = ${X}")

unset(X)
message("[1] X = ${X}")

unset(X CACHE)
message("[2] X = ${X}")

option(Y "Y option" ON)
set(Y OFF)
message("[0] Y = ${Y}")

unset(Y)
message("[1] Y = ${Y}")

unset(Y CACHE)
message("[2] Y = ${Y}")
