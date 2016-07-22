cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(a "xyz")

set(b "${a}_321")
set(${a}_1 "456")
set(variable_${a} "${a} + ${b} + 155")

message("b: '${b}'")
message("xyz_1: '${xyz_1}'")
message("variable_xyz: '${variable_xyz}'")
