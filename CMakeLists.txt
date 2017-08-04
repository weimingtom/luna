cmake_minimum_required(VERSION 2.6)

project(luna)

if(MSVC)
set(CMAKE_CXX_FLAGS
    )
else()
set(CMAKE_CXX_FLAGS
    "-std=c++11 -Wall -Wextra -Wno-unused-parameter -O2"
    )
endif()

set(EXECUTABLE_OUTPUT_PATH "${PROJECT_BINARY_DIR}/bin")
set(LIBRARY_OUTPUT_PATH "${PROJECT_BINARY_DIR}/lib")

add_subdirectory(luna)
add_subdirectory(unittests)
