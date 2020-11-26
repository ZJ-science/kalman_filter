cmake_minimum_required(VERSION 2.6)
project(kalman_filter)

add_executable(kalman_filter main.cpp)
#include_directories("user/local/include/eigen3")
#target_link_libraries(kalman_filter eigen3)
add_subdirectory(user)

target_link_libraries(kalman_filter kf)

install(TARGETS kalman_filter RUNTIME DESTINATION bin)



