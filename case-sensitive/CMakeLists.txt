cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(a "123")
set(b "567")
set(aBc "333")

set(A "321")
set(B "765")
set(ABc "777")

message("a: ${a}")
message("b: ${b}")
message("aBc: ${aBc}")

message("A: ${A}")
message("B: ${B}")
message("ABc: ${ABc}")
