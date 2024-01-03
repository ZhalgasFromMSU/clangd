cmake_minimum_required(VERSION 3.28)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

project(example CXX)

add_executable(main
  main.cpp
)

target_sources(main
PUBLIC FILE_SET modules TYPE CXX_MODULES FILES
  some_module.cpp
)
