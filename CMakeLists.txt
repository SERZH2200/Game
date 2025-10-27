cmake_minimum_required(VERSION 3.28.3)
project(Game)

set(CMAKE_CXX_STANDARD 23)

find_package(SDL3 REQUIRED)

add_executable(Game main.cpp)

target_link_libraries(Game PRIVATE ${SDL3_LIBRARIES})
