cmake_minimum_required(VERSION 3.28)
project(RubiksCubeSolver)

set(CMAKE_CXX_STANDARD 17)

set(Headers RubiksCube.h)

add_executable(RubixCubeSolver ${PROJECT_SOURCE_DIR}/ main.cpp RubiksCube.cpp
        RubiksCube.h
        RubiksCube3dArray.cpp
        RubiksCube3dArray.cpp)


