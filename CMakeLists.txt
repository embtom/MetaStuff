project (exampleJason)
cmake_minimum_required(VERSION 3.10)

set (CMAKE_CXX_STANDARD 17)
SET (SOURCE example/main.cpp
            example/StringCast.cpp)

add_executable(${PROJECT_NAME} ${SOURCE})
target_include_directories(${PROJECT_NAME} PRIVATE example/nlohmann_json include include/detail)
