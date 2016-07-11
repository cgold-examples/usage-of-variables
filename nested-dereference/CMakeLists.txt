cmake_minimum_required(VERSION 2.8)
project(foo)

foreach(lang C CXX)
  message("Compiler for language ${lang}: ${CMAKE_${lang}_COMPILER}")
  foreach(build_type DEBUG RELEASE RELWITHDEBINFO MINSIZEREL)
    message("Flags for language ${lang} + build type ${build_type}: ${CMAKE_${lang}_FLAGS_${build_type}}")
  endforeach()
endforeach()
