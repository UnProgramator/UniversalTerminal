﻿# CMakeList.txt : CMake project for CMakeProject1, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
add_executable (UniversalTerminal "main.cpp" "UniversalTerminal.h" "utilities.cpp" "utilities.h" 
				"execute.cpp" "execute.h" "dir.cpp" "dir.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET UniversalTerminal PROPERTY CXX_STANDARD 20)
endif()


# TODO: Add tests and install targets if needed.
