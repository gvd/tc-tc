cmake_minimum_required(VERSION 3.8)
project(tc_tc)

set(CMAKE_CXX_STANDARD 11)

add_subdirectory(tc-geo)
include_directories(.)

set(SOURCE_FILES main.cpp)
add_executable(tc_tc ${SOURCE_FILES})
target_link_libraries(tc_tc tc_geo)