cmake_minimum_required(VERSION 3.0)

project(byteorder C)

list(APPEND inc_files "include/byteorder/byteorder.h")
set(inc_dir "${CMAKE_CURRENT_SOURCE_DIR}/include")

add_library(byteorder INTERFACE)
set_target_properties(byteorder PROPERTIES
	INTERFACE_INCLUDE_DIRECTORIES "${inc_dir}")
