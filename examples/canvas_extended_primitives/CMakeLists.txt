cmake_minimum_required(VERSION 2.8.11)
project(canvas_extended_example)

if(NOT MSVC)
	add_definitions(-Wall)
	add_definitions(-pedantic)
	add_definitions(-Werror)
endif()

add_executable(sgfx_canvas_extended main.cpp)
set_target_properties(sgfx_canvas_extended PROPERTIES CXX_STANDARD 17 CXX_STANDARD_REQUIRED ON)

# add_subdirectory(../../sgfx build)
target_link_libraries(sgfx_canvas_extended sgfx)
