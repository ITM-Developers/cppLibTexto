cmake_minimum_required(VERSION 3.14)

project(LibTexto LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(LibTexto SHARED
  LibTexto_global.h
  libtexto.cpp
  libtexto.hpp
)

target_compile_definitions(LibTexto PRIVATE LIBTEXTO_LIBRARY)
