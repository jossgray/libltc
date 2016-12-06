cmake_minimum_required(VERSION 2.8.9)
project(libltc)

set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)

file(GLOB SOURCES "src/*.h")
file(GLOB SOURCES "src/*.c")

add_library(libltc SHARED ${SOURCES})
add_library(libltc_static STATIC ${SOURCES})
