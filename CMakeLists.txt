cmake_minimum_required(VERSION "3.16")

project(HelloOpenGL)

find_package(glfw3 CONFIG REQUIRED)
find_package(glad CONFIG REQUIRED)
add_executable(window window.cpp)
target_link_libraries(window PRIVATE glfw glad::glad)
