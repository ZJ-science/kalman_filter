cmake_minimum_required(VERSION 2.6)

include_directories(${CMAKE_BINARY_DIR})

include_directories(${PROJECT_SOURCE_DIR})
#include_directories("usr/local/include/eigen3")
file(GLOB sources "include/*.h" "src/*.cpp")

add_library(kf SHARED ${sources})

#target_link_libraries(kf eigen3)


