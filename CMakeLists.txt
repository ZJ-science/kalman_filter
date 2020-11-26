cmake_minimum_required(VERSION 2.6)
project(kalman_filter)

add_executable(kalman_filter main.cpp)

install(TARGETS kalman_filter RUNTIME DESTINATION bin)
