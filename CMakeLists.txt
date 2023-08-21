# 最低要求版本
cmake_minimum_required(VERSION 3.16.3)
# 项目名
project(cppHelloWorld)

#进入子目录hw，并且执行CMakeLists.txt
add_subdirectory(hw)

add_executable(main main.cpp)

#指定头文件搜索目录
target_include_directories(main PUBLIC world)

#添加库的链接
target_link_libraries(main PUBLIC helloLib)