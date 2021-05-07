cmake_minimum_required(VERSION 3.4)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

project(formatter_ex)

include_directories(/home/helga/lab03/lab03/formatter_lib)
add_subdirectory(/home/helga/lab03/lab03/formatter_lib formatter)

add_library(formatter_ex STATIC formatter_ex.cpp)

target_link_libraries(formatter_ex formatter)
