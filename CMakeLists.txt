cmake_minimum_required(VERSION 3.31)
project(
    Glad2
    DESCRIPTION "Multi-Langugae GL Loader-Generator."
    LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 23)
set(LIBRARY "Glad2")

project(${LIBRARY})

add_library(${LIBRARY} include/glad/gl.h src/gl.c include/KHR/khrplatform.h)
target_include_directories(${LIBRARY} PUBLIC include/)
