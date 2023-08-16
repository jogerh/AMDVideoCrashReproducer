cmake_minimum_required(VERSION 3.16)
project(AMDVideoCrashReproducer)
set(CMAKE_CXX_STANDARD 17)

add_executable(AMDVideoCrashReproducer main.cpp)
target_compile_options(AMDVideoCrashReproducer PUBLIC "-W4")