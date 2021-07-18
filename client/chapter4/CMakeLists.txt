
cmake_minimum_required(VERSION 3.0)

message(STATUS "Configuring chapter4")

project(chapter4)

set(SOURCE_FILES
	./src/main.cpp
	)

add_executable(${PROJECT_NAME} ${SOURCE_FILES})

target_link_libraries(${PROJECT_NAME} glad glfw glm shaderlib)
