cmake_minimum_required(VERSION 3.10)
project(MyTBBProject)
# Specify the TBB installation root
set(CMAKE_PREFIX_PATH "${CMAKE_SOURCE_DIR}/intel/tbb/latest/;${CMAKE_PREFIX_PATH}")

find_package(TBB REQUIRED)

add_executable(example main.cpp)
target_link_libraries(example TBB::tbb)
