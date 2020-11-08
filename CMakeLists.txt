cmake_minimum_required(VERSION 3.17)

project(boost_guide)

set(CMAKE_CXX_STANDARD 14)

add_compile_options("$<$<C_COMPILER_ID:MSVC>:/utf-8>")
add_compile_options("$<$<CXX_COMPILER_ID:MSVC>:/utf-8>")

find_package(Boost REQUIRED)
INCLUDE_DIRECTORIES( ${Boost_INCLUDE_DIR} )
LINK_DIRECTORIES(${Boost_LIBRARY_DIR})

include_directories(common)

add_subdirectory(common)
add_subdirectory(date_time)

