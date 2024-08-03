

make_minimum_required(VERSION 3.20)

project(HelloApp VERSION 1.0)

find_package(HelloLibrary REQUIRED PATHS ../library/install)

add_executable(HelloApp main.cpp)

target_link_libraries(HelloApp PRIVATE HelloLibrary)
