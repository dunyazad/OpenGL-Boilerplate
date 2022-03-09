# CMakeLists.txt for source

add_executable(${PROJECT_NAME} "main.c")

target_link_libraries(${PROJECT_NAME} PUBLIC glfw glad)
