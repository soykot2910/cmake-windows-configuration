cmake_minimum_required(VERSION 3.20.0)

# change this to your path
set(CMAKE_TOOLCHAIN_FILE "F:/c++/vcpkg/scripts/buildsystems/vcpkg.cmake")

project(demo)

add_executable(${PROJECT_NAME} main.cpp)

# set(CMAKE_PREFIX_PATH "E:/src/vcpkg/installed/x64-windows/share")
find_package(fmt CONFIG REQUIRED)
target_link_libraries(${PROJECT_NAME} PRIVATE fmt::fmt)