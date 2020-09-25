cmake_minimum_required(VERSION 3.16)

project(PleaseChangeMe
        VERSION 0.0.1)

set(CMAKE_CXX_STANDARD  20)

option(TEST "Enable testing" OFF)

# Add external dependencies
add_subdirectory(ext)

# Add project sources
add_subdirectory(src)

if (TEST)
    add_subdirectory(test)
endif()