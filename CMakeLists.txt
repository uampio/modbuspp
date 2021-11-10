cmake_minimum_required(VERSION 3.1)

project(modbuspp VERSION 0.3 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 14)

if(WIN32)
    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall")
else()
    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Werror")
endif()

add_subdirectory(include)