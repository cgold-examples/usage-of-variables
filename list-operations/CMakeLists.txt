cmake_minimum_required(VERSION 2.8)
project(foo NONE)

set(l0 "a;b;c")
set(l1 "a" "b;c")
set(l2 "a" "b c")

list(LENGTH l0 l0_len)
list(LENGTH l1 l1_len)
list(LENGTH l2 l2_len)

message("length of '${l0}' (l0) = ${l0_len}")
message("length of '${l1}' (l1) = ${l1_len}")
message("length of '${l2}' (l2) = ${l2_len}")

list(GET l1 2 l1_2)
message("l1[2] = ${l1_2}")

message("Removing first item from l1 list: '${l1}'")
list(REMOVE_AT l1 0)
message("l1 = '${l1}'")
