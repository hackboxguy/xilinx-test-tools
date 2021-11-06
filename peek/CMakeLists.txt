cmake_minimum_required(VERSION 2.8.9)
set(COMPONENT_NAME peek)  #set the name of the binary
project(${COMPONENT_NAME})
file(GLOB SOURCES "*.c")
add_executable(${COMPONENT_NAME} ${SOURCES})
install(TARGETS ${COMPONENT_NAME} DESTINATION bin)
#for cross compiling
#cmake -H. -BOutput -DCMAKE_TOOLCHAIN_FILE=/path/to/toolchain-arm-backup.cmake -DCMAKE_INSTALL_PREFIX=/home/user/tmp/
#cmake --build Output -- all
#cmake --build Output -- install

#for local compiling
#cmake -H. -BOutput
#cmake --build Output -- all

