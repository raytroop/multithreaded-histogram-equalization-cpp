# project name
PROJECT(hist_equal)
# requirement of cmake version
cmake_minimum_required(VERSION 3.10)

# find required opencv
find_package(OpenCV REQUIRED)
# directory of opencv headers
include_directories(${OpenCV_INCLUDE_DIRS})
# name of executable file and path of source file
add_executable(hist_equal hist_equal.cpp)
# opencv libraries
target_link_libraries(hist_equal ${OpenCV_LIBS} pthread)