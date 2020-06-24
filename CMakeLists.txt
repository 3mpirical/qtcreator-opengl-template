cmake_minimum_required(VERSION 3.5)

project(qtcreator-opengl LANGUAGES CXX)

include_directories("${CMAKE_SOURCE_DIR}/include")

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_executable(qtcreator-opengl
    # Main
    src/main.cpp

    # Headers

    # Implementations
)

target_link_libraries(qtcreator-opengl
    GL
    GLU
    glfw3
    X11
    Xrandr
    pthread
    Xi
    dl
    Xinerama
    Xcursor
    GLEW
)
