cmake_minimum_required(VERSION 3.21)

project(Assign2)

find_package(Qt6 REQUIRED COMPONENTS Core)

set(CMAKE_AUTOMOC ON)

add_executable(my_app main.cpp player.cpp include/player.hpp)

target_include_directories(my_app PRIVATE include)
target_link_libraries(my_app PRIVATE Qt6::Core)
