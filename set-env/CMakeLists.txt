cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(ENV{USERNAME} "Jane Doe")
message("Environment variable USERNAME: $ENV{USERNAME}")
