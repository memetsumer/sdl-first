cmake_minimum_required(VERSION 3.0)
project(MySDLProject C)

# Find SDL2 library
find_package(SDL2 REQUIRED)

# Add your source file
add_executable(my_executable main.c)

# Link against SDL2 libraries
target_link_libraries(my_executable ${SDL2_LIBRARIES})

# Include SDL2 include directories
include_directories(${SDL2_INCLUDE_DIRS})
