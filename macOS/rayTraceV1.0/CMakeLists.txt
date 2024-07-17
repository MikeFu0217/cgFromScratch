cmake_minimum_required(VERSION 3.0.0)
set(NAME rayTrace)
project(${NAME} VERSION 1.0)

# 使用 C++ 17 标准
set(CMAKE_CXX_STANDARD 17)

# 设置代码文件
set(SRC_DIR ${PROJECT_SOURCE_DIR}/src/)

# 添加头文件
set(HEADER_DIR ${PROJECT_SOURCE_DIR}/include/)
include_directories(${HEADER_DIR})

# 执行编译命令
set(SOURCES ${SRC_DIR}main.cpp)
add_executable(${NAME} ${SOURCES})