cmake_minimum_required(VERSION 3.17)
project(PathFinding)

set(CMAKE_CXX_STANDARD 17)
set(SOURCE_FILES src/main.cpp)


include_directories(${PROJECT_SOURCE_DIR}/Include/GLFW)
link_directories(${PROJECT_SOURCE_DIR}/Lib/lib-mingw)

add_executable(PathFinding src/main.cpp)


target_link_libraries(PathFinding glfw3 gdi32 opengl32)