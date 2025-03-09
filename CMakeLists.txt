cmake_minimum_required(VERSION 3.13)

set(target circle_buffer_lib)
project(${target} C)

add_library(${target} INTERFACE)

target_sources(${target} INTERFACE
	src/cbuffer.c
)

target_include_directories(${target} INTERFACE
	src
)
