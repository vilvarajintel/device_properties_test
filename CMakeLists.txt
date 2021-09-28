cmake_minimum_required(VERSION 3.8)

project(test_device_properites)

add_definitions(-std=c++17)

# Add source to this project's executable.
add_executable (test_device_properites "main.cpp")

target_link_directories(test_device_properites PUBLIC /home/tvilvara/NEO_embargo/neo/build_clang10/bin)
target_link_libraries (test_device_properites PUBLIC pthread)
target_link_libraries (test_device_properites PUBLIC ze_intel_gpu)
