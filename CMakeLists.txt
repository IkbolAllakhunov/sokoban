cmake_minimum_required(VERSION 3.27)
project(final LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Qt6 REQUIRED COMPONENTS Widgets)
qt_standard_project_setup()

qt_add_executable(final main.cpp shape.h circle.h)
target_link_libraries(final PRIVATE Qt6::Widgets)



