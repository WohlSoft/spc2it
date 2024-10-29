cmake_minimum_required(VERSION 3.5)
project(spc2it)

set(spc2it_sources
	src/emu.cpp
	src/it.cpp
	src/main.cpp
	src/sound.cpp
	src/spc700.cpp

	src/emu.h
	src/it.h
	src/sneese_spc.h
	src/sound.h
	src/spc2ittypes.h
)

add_executable(spc2it ${spc2it_sources})
target_include_directories(spc2it PRIVATE src)

target_link_libraries(spc2it m)
