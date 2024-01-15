cmake_minimum_required(VERSION 3.8)

project(
	CMakeProject_Template_1
	VERSION 0.0.1
	DESCRIPTION "CMake Project Template ver. 1 for future projects"
	LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)

# Library code
add_subdirectory(core)

# Executable(s)
add_subdirectory(apps)