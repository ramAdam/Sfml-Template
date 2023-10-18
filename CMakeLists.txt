cmake_minimum_required(VERSION 3.0)

project(HelloWorldSFML)

# Find SFML
find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

# Add the executable
add_executable(HelloWorld Game.cpp)

# Link SFML
target_link_libraries(HelloWorld PRIVATE sfml-graphics sfml-window sfml-system)
