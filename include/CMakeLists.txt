cmake_minimum_required(VERSION 3.10)
project(Assign2)

find_package(Boost REQUIRED COMPONENTS filesystem)
find_package(Qt6 REQUIRED COMPONENTS Core)

set(CMAKE_AUTOMOC ON)

add_executable(my_app main.cpp player.cpp player.hpp)
target_link_libraries(my_app PRIVATE Qt6::Core)
