cmake_minimum_required(VERSION 3.10)
project(bbb_app)

include_directories(include)

add_library(core STATIC src/add.cpp)

add_executable(bbb_app src/main.cpp)
target_link_libraries(bbb_app core)

add_executable(unit_test tests/test_add.cpp)
target_link_libraries(unit_test core)
