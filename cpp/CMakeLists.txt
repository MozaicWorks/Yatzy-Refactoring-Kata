cmake_minimum_required(VERSION 3.7)
project(cpp)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Werror -O")

set(SOURCE_FILES
        yatzy.cpp
        yatzy.hpp
        yatzy.tests.cpp)

add_executable(run.tests ${SOURCE_FILES})
add_custom_target(runAllTests ALL COMMAND run.tests)