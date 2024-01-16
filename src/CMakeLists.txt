cmake_minimum_required(VERSION 3.18.0)

set(CMAKE_WINDOWS_EXPORT_ALL_SYMBOLS ON)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/../bin)

project(RacingDiplom VERSION 1.0)

add_subdirectory(TSlib)
include_directories(TSlib)

set(SOURCE_EXE Racing.cpp aSession.cpp)
add_executable(${PROJECT_NAME} ${SOURCE_EXE})
target_link_libraries(${PROJECT_NAME} TS)
