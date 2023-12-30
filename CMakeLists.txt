cmake_minimum_required(VERSION 3.26)
project(string_binary)

set(CMAKE_CXX_STANDARD 17)

# Find libxml2 package
find_package(LibXml2 REQUIRED)
include_directories(${LIBXML2_INCLUDE_DIR})

# Add your executable
add_executable(string_binary main.cpp)

# Link libxml2
target_link_libraries(string_binary ${LIBXML2_LIBRARIES})
