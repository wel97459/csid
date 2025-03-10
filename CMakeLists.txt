cmake_minimum_required(VERSION 3.10)

project(csid)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(SDL2 REQUIRED)
add_executable(csidl csid-light.c)
target_link_libraries(csidl SDL2::SDL2 m)

add_executable(csid csid.c)
target_link_libraries(csid SDL2::SDL2 m)

