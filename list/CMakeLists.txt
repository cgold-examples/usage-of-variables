cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(l0 a b c)
set(l1 a;b;c)
set(l2 "a b" "c")
set(l3 "a;b;c")
set(l4 a "b;c")

message("l0 = 'a' + 'b' + 'c' = '${l0}'")
message("l1 = 'a;b;c' = '${l1}'")
message("l2 = 'a b' + 'c' = '${l2}'")
message("l3 = \"'a;b;c'\" = '${l3}'")
message("l4 = 'a' + 'b;c' = '${l4}'")

message("print by message: " ${l3})
message("print by message: " "a" "b" "c")
