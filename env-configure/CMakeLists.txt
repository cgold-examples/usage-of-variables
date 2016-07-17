cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

set(ENV{ABC} "123")

message("Environment variable ABC: $ENV{ABC}")

add_custom_target(
    foo
    ALL
    "${CMAKE_COMMAND}" -P "${CMAKE_CURRENT_LIST_DIR}/script.cmake"
)
