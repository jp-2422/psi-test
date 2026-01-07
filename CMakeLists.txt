cmake_minimum_required(VERSION 3.5)

project(psi-test C)

set(CMAKE_COLOR_MAKEFILE OFF)
set(CMAKE_VERBOSE_MAKEFILE ON)

set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wall")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wextra")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Werror")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wshadow")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wwrite-strings")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wmissing-prototypes")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -Wbad-function-cast")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pedantic")
set(CMAKE_C_FLAGS "${CMAKE_C_FLAGS} -pedantic-errors")

add_executable(psi-test
	psi-test.c
)

install(TARGETS psi-test)

