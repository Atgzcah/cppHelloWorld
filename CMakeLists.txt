cmake_minimum_required(VERSION 3.16.3)
project(cppHelloWorld)

add_executable(main main.cpp hw/hello.cpp)
target_include_directories(main PUBLIC world)