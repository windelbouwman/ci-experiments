
cmake_minimum_required(VERSION 3.20)

project(HelloLibrary VERSION 1.0)


add_library(hello SHARED HelloLib.cpp)

install(TARGETS hello)
