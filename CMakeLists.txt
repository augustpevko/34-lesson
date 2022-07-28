cmake_minimum_required(VERSION 3.0.0)
project(1-task VERSION 0.1.0)

set(CMAKE_PREFIX_PATH "/home/pavel/Qt/6.3.1/gcc_64/lib/cmake/")

find_package(Qt6 COMPONENTS Core Gui Widgets REQUIRED)

add_executable(1-task main.cpp)

target_link_libraries(1-task Qt6::Widgets Qt6::Core Qt6::Gui)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
