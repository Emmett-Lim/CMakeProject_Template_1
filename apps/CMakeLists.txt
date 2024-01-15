cmake_minimum_required(VERSION 3.8)

project(
	MyApp
	VERSION 0.0.1
	DESCRIPTION "CMake Project Template ver. 1 for future projects"
	LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)

add_executable(${PROJECT_NAME} src/app.cpp)

target_link_libraries(${PROJECT_NAME} core)