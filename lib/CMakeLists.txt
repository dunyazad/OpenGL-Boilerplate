# CMakeLists.txt for libraries

# glad
set(GLAD_LIB_NAME "glad")
set(GLAD_SRC_PATH "${GLAD_LIB_NAME}/src")
set(GLAD_INC_PATH "${GLAD_LIB_NAME}/include")

add_library(${GLAD_LIB_NAME} STATIC "${GLAD_SRC_PATH}/glad.c")

target_include_directories(${GLAD_LIB_NAME} PUBLIC "${GLAD_INC_PATH}")


# glfw
set(GLFW_LIB_NAME "GLFW")
set(GLFW_INC_PATH ${GLFW_LIB_NAME}/include)

set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)

add_subdirectory(glfw)
