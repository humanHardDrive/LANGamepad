cmake_minimum_required(VERSION 3.3)

include(pico_sdk_import.cmake)

project(pico-test)

pico_sdk_init()

add_executable(pico-test
	pico-test.c
)

target_link_libraries(pico-test pico_stdlib)

pico_add_extra_outputs(pico-test)
