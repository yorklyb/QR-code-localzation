cmake_minimum_required(VERSION 2.8)

project(QRCODE)

add_executable(QRCODE QRCODE.cpp)


find_package(OpenCV REQUIRED)

set(CMAKE_CXX_FLAGS "-std=c++11")


# 链接OpenCV库
target_link_libraries(QRCODE ${OpenCV_LIBS})

#add_executable(undistortImage undistortImage.cpp)

