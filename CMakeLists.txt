cmake_minimum_required(VERSION 2.8.9)
set(PROJECT_NAME xilinx-test-tools)
project(${PROJECT_NAME})
add_subdirectory(peek)
add_subdirectory(poke)
add_subdirectory(gpio-demo)
#cmake -H. -BOutput
#cmake --build Output -- all -j$(nproc)
######or#########
#cmake -H. -BOutput -DCMAKE_INSTALL_PREFIX=~/tmp/
#cmake --build Output -- install -j$(nproc)
