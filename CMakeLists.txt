cmake_minimum_required(VERSION 3.11)
project(TestTdLib)

find_package(Td REQUIRED)
add_executable(example td_example.cpp)
target_link_libraries(example PRIVATE Td::TdStatic)
