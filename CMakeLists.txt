cmake_minimum_required(VERSION 3.20.0)
project(benchmark)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(BENCHMARK_DOWNLOAD_DEPENDENCIES ON)

include(FetchContent)
FetchContent_Declare(
  benchmark
  GIT_REPOSITORY https://github.com/google/benchmark.git
  GIT_TAG v1.9.4)
FetchContent_MakeAvailable(benchmark)

add_subdirectory(src)
