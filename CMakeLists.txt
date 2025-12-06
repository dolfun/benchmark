cmake_minimum_required(VERSION 3.20.0)
project(benchmark)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(GOOGLETEST_PATH "${CMAKE_SOURCE_DIR}/extern/googletest")
add_subdirectory(extern/benchmark)

add_subdirectory(src)
