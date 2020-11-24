CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(asio-test)

set (DEBUG_SYMBOL "-g")
set (CMAKE_CXX_FLAGS -pipe -Wall -W -std=gnu++14 -lpthread)
set (CMAKE_C_FLAGS -pipe -Wall -W -std=gnu++14 -lpthread)

# 更改生成目录
set (EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/product/bin)
# 更改lib生成目录
set (LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/product/lib)
message ("current platform: ${CMAKE_SYSTEM_NAME}")

# 设置头文件路径
include_directories ("${PROJECT_SOURCE_DIR}/asio/include")

add_subdirectory(example)