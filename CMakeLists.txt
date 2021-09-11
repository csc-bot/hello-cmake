cmake_minimum_required(VERSION 3.16)

project(
  HelloCmake
  VERSION 1.0
  LANGUAGES CXX
)

list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_LIST_DIR}/cmake)

add_subdirectory(external)
add_subdirectory(src)
