
cmake_minimum_required(VERSION 3.7)
project(Hello)
list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_LIST_DIR}/.cdep/modules")

find_package(boost REQUIRED)
if(NOT BOOST_FOUND)
  message(error "'BOOST_FOUND' was not defined by the module")
endif()

add_executable(hello hello.cpp)
