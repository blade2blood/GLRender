
cmake_minimum_required(VERSION 3.0)

message(STATUS "Configuring shaderlib")

project(shaderlib)

set(SOURCE_FILES
	./src/gl_shader.cpp
	)

add_library(${PROJECT_NAME} STATIC ${SOURCE_FILES})

target_link_libraries(${PROJECT_NAME} glad glfw glm)

target_include_directories(${PROJECT_NAME} PUBLIC ./include)
