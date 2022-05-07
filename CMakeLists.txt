# refer to the root source directory of the project as ${DEMO_SOURCE_DIR} and
# to the root binary directory of the project as ${DEMO_BINARY_DIR}.

cmake_minimum_required(VERSION 3.10)
project (DEMO)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_subdirectory(SPADS)

add_executable (demo demo.cpp)
target_link_libraries (demo LINK_PUBLIC SPADS)