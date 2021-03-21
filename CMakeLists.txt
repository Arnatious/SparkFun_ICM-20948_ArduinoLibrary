cmake_minimum_required(VERSION 3.19)

project(ICM20948 C CXX ASM)

add_library(ICM20948 INTERFACE)
target_sources(ICM20948 INTERFACE
    ${CMAKE_CURRENT_LIST_DIR}/src/util/ICM_20948_C.c
)
target_include_directories(ICM20948 INTERFACE ${CMAKE_CURRENT_LIST_DIR}/src/util)
