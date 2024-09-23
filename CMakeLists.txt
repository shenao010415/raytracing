cmake_minimum_required(VERSION 3.30.3)

project(HelloWorld
    VERSION 1.0.0
    DESCRIPTION "A simple Hello World program"
    HOMEPAGE_URL "https://github.com/shenao010415/raytracing"
    LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_SOURCE_DIR}/bin)
set(Hello_Dir ${CMAKE_CURRENT_SOURCE_DIR}/src/hello)
set(World_Dir ${CMAKE_CURRENT_SOURCE_DIR}/src/world)

add_subdirectory(src)