set(CMAKE_VERBOSE_MAKEFILE 1)
cmake_minimum_required(VERSION 2.8)
PROJECT(CppTemplate CXX)

enable_testing()

#
find_package(Boost)
if(Boost_FOUND)
  include_directories(${Boost_INCLUDE_DIRS})
endif()

if(NOT CMAKE_CXX_COMPILER)
  set(CMAKE_CXX_COMPILER clang++)
endif()

include_directories("${PROJECT_SOURCE_DIR}")

add_definitions(-std=c++1y -Wall)

add_subdirectory(src)
add_subdirectory(test)
