
cmake_minimum_required(VERSION 3.7)
project(Hello)
list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/.cdep/modules")
find_package(boost REQUIRED)
include_directories(${LOW_LEVEL_STATISTICS_INCLUDE_DIRS})
add_executable(hello hello.cpp)
