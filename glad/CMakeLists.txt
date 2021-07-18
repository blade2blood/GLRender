
cmake_minimum_required(VERSION 3.0)

project(glad)

message(STATUS "Configuring glad")

set(HEADER_FILES
	./include/glad/glad.h
	./include/KHR/khrplatform.h
	)

set(SOURCE_FILES
	./src/glad.c
	)

add_library(${PROJECT_NAME} STATIC ${HEADER_FILES} ${SOURCE_FILES})

target_include_directories(${PROJECT_NAME} PUBLIC ./include)