cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

unset(ENV{USERNAME})
message("Environment variable USERNAME: $ENV{USERNAME}")
