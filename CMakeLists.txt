set(CMAKE_MINIMUM_VERSION $ENV{CMAKE_MINIMUM_VERSION})
cmake_minimum_required(VERSION ${CMAKE_MINIMUM_VERSION}) 

message(STATUS "CMake version : ${CMAKE_VERSION}")
message(STATUS "CMake version required : ${CMAKE_MINIMUM_VERSION}")

project(BlackHole LANGUAGES C CXX ASM)

# Compiler check
if(NOT "${CMAKE_C_COMPILER_ID}" STREQUAL "${CMAKE_COMPILER}")
  message(FATAL_ERROR "${CMAKE_C_COMPILER_ID} is not ${CMAKE_COMPILER}")
endif()



