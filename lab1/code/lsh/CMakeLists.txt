cmake_minimum_required(VERSION 3.5)
project(lsh)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -O2 -Wall -Wextra -Werror")

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
add_library(lsh src/a.cpp src/b.cpp src/c.cpp)

install(TARGETS lsh DESTINATION lib)
install(DIRECTORY include/lsh DESTINATION include)