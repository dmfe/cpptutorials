cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDART 17)
set(CMAKE_CXX_STANDART_REQUIRED ON)

project(sort VERSION 1.0)

file(GLOB_RECURSE SRC_FILES src/*.cpp)
add_executable(sort ${SRC_FILES})
target_include_directories(sort PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}/include)
