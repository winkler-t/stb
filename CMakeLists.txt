cmake_minimum_required(VERSION 3.10)

# Project name
project(stb)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_C_STANDARD 17)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${PROJECT_SOURCE_DIR}/bin")

file(GLOB_RECURSE SOURCE_FILES ./*.cpp ./*.c)
file(GLOB_RECURSE HEADER_FILES ./*.hpp ./*.h)

# stb library
add_executable(stb ${SOURCE_FILES} ${HEADER_FILES})
source_group("Source Files" FILES ${SOURCE_FILES})
source_group("Header Files" FILES ${HEADER_FILES})

