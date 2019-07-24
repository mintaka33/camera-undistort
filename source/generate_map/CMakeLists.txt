cmake_minimum_required(VERSION 2.8)

project(remap)

set (SOURCE_FILES 
    remap.cpp
)

include_directories (remap C:\data\code\opencv\build2\install\include)

link_directories(C:\data\code\opencv\build2\install\x64\vc15\lib)

add_executable(remap ${SOURCE_FILES})
target_link_libraries(remap opencv_imgproc410d.lib opencv_calib3d410d.lib)