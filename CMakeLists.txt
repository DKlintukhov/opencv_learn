cmake_minimum_required(VERSION 3.23)

set(PROJECT_NAME opencv_learn)

project(${PROJECT_NAME})

add_executable(${PROJECT_NAME} main.cpp)

# opencv
find_package(OpenCV REQUIRED)
message(OpenCV)
include_directories(${OpenCV_INCLUDE_DIRS})
target_link_libraries(${PROJECT_NAME} ${OpenCV_LIBS})
