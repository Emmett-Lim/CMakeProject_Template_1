cmake_minimum_required(VERSION 3.8)

project(
	MyCore
	VERSION 0.0.1
	DESCRIPTION "CMake Project Template ver. 1 for future projects"
	LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)

# Source Files
set(CORE_SOURCE_FILES
	src/core.cpp)

# Header Files
set(CORE_HEADER_FILES
	include/core_include/core.h)

add_library(core STATIC ${CORE_SOURCE_FILES} ${CORE_HEADER_FILES})

target_include_directories(core
	PUBLIC
		$<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
		$<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>
	PRIVATE
		${CMAKE_CURRENT_SOURCE_DIR}
)