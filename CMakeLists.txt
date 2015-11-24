project(strings)
cmake_minimum_required(VERSION 2.8)

SET(CMAKE_CXX_FLAGS_RELEASE "-O2")
SET(CMAKE_BUILD_TYPE Release)
add_definitions("-std=c++11 -static")

FILE(GLOB strings_cc_files src/*.cc)

add_library(strings ${strings_cc_files})
