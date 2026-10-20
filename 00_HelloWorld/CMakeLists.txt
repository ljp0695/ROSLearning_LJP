cmake_minimum_required(VERSION 3.10)
project(00_HelloWorld)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include_directories(${PROJECT_SOURCE_DIR}/include)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)

aux_source_directory(${PROJECT_SOURCE_DIR}/src SRC_LIST)

add_executable(HelloWorld main.cpp ${SRC_LIST})