# CMake configuration for Rubik's Cube Engine

cmake_minimum_required(VERSION 3.10)
project(RubixEngine)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)

# Add source files
set(SOURCES
    RubiksCube.cpp
    RubiksCube1D.cpp
    RubiksCube3d.cpp
    RubiksCubeBitBoard.cpp
)

# Add header files
set(HEADERS
    RubiksCube.h
)

# Create executable
add_executable(RubixEngine ${SOURCES} ${HEADERS})

# Include directories
include_directories(${CMAKE_SOURCE_DIR})