cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(a "Quoted argument")
set(b x-"Unquoted argument")
set(c x"a;b;c")

message("a = '${a}'")
message("b = '${b}'")

message("c =")
foreach(x ${c})
  message("  '${x}'")
endforeach()
