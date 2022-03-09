# CMakeLists.txt for project

cmake_minimum_required(VERSION 3.19)

# Change project name from test to whatever you want
project(OpenGLTest)

# Requires OpenGL 
find_package(OpenGL REQUIRED)

add_subdirectory(lib)
add_subdirectory(src)
