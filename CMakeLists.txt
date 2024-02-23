# tas/CMakeLists.txt
cmake_minimum_required(VERSION 3.10)
set(DCMAKE_EXPORT_COMPILE_COMMANDS ON)
project(TAS_CLIENT)


add_compile_options(-std=c++14 -O3 -g3 -Wall -march=native -fno-omit-frame-pointer)

# tas source files
set(TAS_CLIENT_SRCS 
    tas_client.cpp
)

add_executable(tas_client ${TAS_CLIENT_SRCS} )

