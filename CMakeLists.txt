cmake_minimum_required (VERSION 3.31)
project (julieGL)
find_package(glfw3 3.4 REQUIRED)
find_package(OpenGL REQUIRED)

#include_directories( ${OPENGL_INCLUDE_DIRS}  ${GLFW_INCLUDE_DIRS} )

# target_link_libraries(testas ${OPENGL_LIBRARIES} ${GLFW_LIBRARY} )


add_executable(julieGL
        main.cpp
)

include_directories(
        includes/
)

target_link_libraries(julieGL glfw)
