cmake_minimum_required(VERSION 3.10)
project(bbb_app)

# Core library
add_library(core src/add.cpp)
include_directories(include)

# Main app
add_executable(bbb_app src/main.cpp)
target_link_libraries(bbb_app core)

# Unit test
add_executable(unit_test tests/test_add.cpp)
target_link_libraries(unit_test core)
