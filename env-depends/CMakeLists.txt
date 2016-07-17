cmake_minimum_required(VERSION 2.8)
project(foo)

set(target_name "$ENV{ABC}-tgt")
add_executable("${target_name}" foo.cpp)
