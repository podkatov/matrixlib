cmake_minimum_required(VERSION 3.23)
project(Matrix)

set(CMAKE_CXX_STANDARD 17)

set(SOURCE_FILES main.cpp)
add_executable(src_run ${SOURCE_FILES})

include_directories(Matrix_lib)
add_subdirectory(Matrix_lib)

target_link_libraries(src_run Matrix_lib)

add_subdirectory(Matrix_tests)
