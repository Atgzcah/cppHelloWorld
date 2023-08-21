# 最低要求版本
cmake_minimum_required(VERSION 3.16.3)
# 项目名
project(hello)
# 设置变量HELLO_SRC，值为${CMAKE_CURRENT_SOURCE_DIR}/hello.cpp，其中{CMAKE_CURRENT_SOURCE_DIR}为内置变量
set(HELLO_SRC ${CMAKE_CURRENT_SOURCE_DIR}/hello.cpp)
# 将变量HELLO_SRC设为helloLib的动态库，其中SHARED意为动态库
add_library(helloLib SHARED ${HELLO_SRC})