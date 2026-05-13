cmake_minimum_required(VERSION 3.15)
project(warframe-api-helper)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_subdirectory(Soup)

add_executable(warframe-api-helper main.cpp)
target_link_libraries(warframe-api-helper PRIVATE soup)
