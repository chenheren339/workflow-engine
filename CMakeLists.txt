cmake_minimum_required(VERSION 3.8)
project(workflow-engine)

set(CMAKE_CXX_STANDARD 14)

include_directories(include)
file(GLOB_RECURSE  ${PROJECT_NAME}_SRC src/*.cpp)
add_library(${PROJECT_NAME} STATIC ${${PROJECT_NAME}_SRC})

