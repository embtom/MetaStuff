cmake_minimum_required(VERSION 3.10)
project (exampleJason)

set (CMAKE_CXX_STANDARD 17)

add_subdirectory(dependencies)
add_subdirectory(example)


add_library(MetaStuff INTERFACE)
target_include_directories(MetaStuff INTERFACE 
    "include"
    "include/detail"
)


