cmake_minimum_required(VERSION 3.11)

project(Single_linked_list CXX)
set(CMAKE_CXX_STANDARD 17)

if (CMAKE_SYSTEM_NAME MATCHES "^MINGW")
    set(SYSTEM_LIBS -lstdc++)
else()
    set(SYSTEM_LIBS)
endif()

add_executable(single-linked-list main.cpp single-linked-list.h)
