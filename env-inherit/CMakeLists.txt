# Top level CMakeLists.txt

cmake_minimum_required(VERSION 2.8)
project(foo LANGUAGES NONE)

message("Set environment variable")

set(ENV{ABC} "This is ABC")

message("Top level ABC: $ENV{ABC}")

set(level1 "${CMAKE_CURRENT_LIST_DIR}/level1.cmake")

execute_process(
    COMMAND "${CMAKE_COMMAND}" -P "${level1}" RESULT_VARIABLE result
)

if(NOT result EQUAL 0)
  # Error
endif()

message("Unset environment variable")

unset(ENV{ABC})

message("Top level ABC: $ENV{ABC}")

execute_process(
    COMMAND "${CMAKE_COMMAND}" -P "${level1}" RESULT_VARIABLE result
)

if(NOT result EQUAL 0)
  # Error
endif()
