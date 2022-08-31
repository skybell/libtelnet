cmake_minimum_required(VERSION 3.5)

file(GLOB SOURCES *.c)
list(APPEND SOURCES libtelnet.c)

idf_component_register(
	SRCS ${SOURCES}
	INCLUDE_DIRS .
	PRIV_INCLUDE_DIRS .
	)

set_source_files_properties(${SOURCES})
