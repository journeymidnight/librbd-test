cmake_minimum_required(VERSION 3.10)
project(rbd_example)

include_directories('/usr/include/rados')
include_directories('/usr/include/rbd')
link_directories(/usr/lib/x86_64-linux-gnu)

set(CMAKE_CXX_STANDARD 11)

add_executable(rbd_example main.cpp)
target_link_libraries(rbd_example rados)
target_link_libraries(rbd_example rbd)

