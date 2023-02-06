# CMakeLists.txt

cmake_minimum_required(VERSION 3.10)

project(cpp_test) 

set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_BUILD_TYPE Release)

add_executable(cpp_test main.cpp)

target_link_libraries(cpp_test)