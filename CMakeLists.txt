cmake_minimum_required(VERSION 3.16) #Minimal Version CMake
project(Alpha) #Project Name

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_SOURCE_DIR}/bin")
list(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake")

include(AutoCollect)
include(GroupSources)

if( NOT CMAKE_BUILD_TYPE )
	set(CMAKE_BUILD_TYPE "release")
endif()

add_subdirectory(source)
#add_subdirectory(3rd_party)
