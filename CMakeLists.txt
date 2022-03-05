cmake_minimum_required(VERSION 3.21)
project(continous_integration)

set(CMAKE_CXX_STANDARD 14)

include_directories(.)

add_library(A A.cc A.h)

add_executable(main main.cc)
target_link_libraries(main A)
