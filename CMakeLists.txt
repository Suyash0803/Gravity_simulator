cmake_minimum_required(VERSION 3.10)

# Set the project name
project(GravitySimulator)

# Find the FreeGLUT package
find_package(FreeGLUT REQUIRED CONFIG)
find_package(OpenGL REQUIRED)

# Add the executable
add_executable(GravitySimulator main.cpp)

# Link the libraries
target_link_libraries(GravitySimulator FreeGLUT::freeglut_static OpenGL::GL)