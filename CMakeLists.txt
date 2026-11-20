cmake_minimum_required(VERSION 3.21)

project(MacroPlayer)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(
    ${GEODE_SDK}
    ${CMAKE_CURRENT_BINARY_DIR}/geode
)

geode_add_mod(
    custom.macroplayer
    src/main.cpp
)
