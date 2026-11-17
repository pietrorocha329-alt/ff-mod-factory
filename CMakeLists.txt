cmake_minimum_required(VERSION 3.18.1)
project("ffmod" LANGUAGES CXX)

add_library(ffpay SHARED main.cpp)

target_link_libraries(ffpay
    android
    log
    EGL
    GLESv2
)