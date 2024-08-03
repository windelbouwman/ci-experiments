
cmake_minimum_required(VERSION 3.20)

project(HelloLibrary VERSION 1.0)


add_library(hello SHARED HelloLib.cpp)
add_library(hello2 SHARED HelloLib.cpp)

install(TARGETS hello EXPORT HelloLibrary)
install(TARGETS hello2 EXPORT HelloLibrary)

install(EXPORT HelloLibrary)
