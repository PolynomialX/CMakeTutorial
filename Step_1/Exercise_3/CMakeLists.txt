cmake_minimum_required(VERSION 3.10)
# TODO 1: Set the minimum required version of CMake to be 3.10
# Amy project's top most CMakeLists.txt must start
# by specifying a minimum version of CMake
# https://cmake.org/cmake/help/latest/command/cmake_minimum_required.html#command:cmake_minimum_required
# Ok the cmake_min... command must be literally on line 1
# Not just the 'first' command
# TODO 2: Create a project named Tutorial
project(Tutorial)
# TODO 7: Set the project version number as 1.0 in the above project command

# TODO 6: Set the variable CMAKE_CXX_STANDARD to 11
#         and the variable CMAKE_CXX_STANDARD_REQUIRED to True
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# TODO 8: Use configure_file to configure and copy TutorialConfig.h.in to
#         TutorialConfig.h

# TODO 3: Add an executable called Tutorial to the project
# Hint: Be sure to specify the source file as tutorial.cxx
add_executable(Tutorial tutorial.cxx)
# TODO 9: Use target_include_directories to include ${PROJECT_BINARY_DIR}
