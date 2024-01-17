cmake_minimum_required(VERSION 3.20)
project(miniabc)

add_library(miniabc INTERFACE)
add_library(miniabc::miniabc ALIAS miniabc)
target_compile_features(miniabc INTERFACE cxx_std_17)
target_include_directories(miniabc INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)
