cmake_minimum_required(VERSION 3.24.0)

project(App)

add_subdirectory(adder)

add_executable(${PROJECT_NAME} main.cpp)

#target_include_directories(${PROJECT_NAME} PUBLIC adder/)
target_link_libraries(${PROJECT_NAME} adder)