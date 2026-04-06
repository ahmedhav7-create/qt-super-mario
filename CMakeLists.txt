cmake_minimum_required(VERSION 3.10)
project(BoostExample)

find_package(Boost REQUIRED COMPONENTS filesystem)

set(CMAKE_AUTOMOC ON)

add_executable(myapp main.cpp)
add_executable(myapp player.hpp)
target_link_libraries(myapp PRIVATE Boost::filesystem)
