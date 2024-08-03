
cmake_minimum_required(VERSION 3.20)

project(HelloLibrary VERSION 1.0)


add_library(hello SHARED HelloLib.cpp)
add_library(hello2 SHARED HelloLib.cpp)

install(TARGETS hello EXPORT ${PROJECT_NAME}-targets)
install(TARGETS hello2 EXPORT ${PROJECT_NAME}-targets)

install(EXPORT ${PROJECT_NAME}-targets
    DESTINATION ${LIB_INSTALL_DIR}/cmake/${PROJECT_NAME})

