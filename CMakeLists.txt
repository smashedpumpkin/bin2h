cmake_minimum_required(VERSION 3.13)

# set the project name
project(bin2h)

# add the executable
add_executable(bin2h bin2h.cpp)

if(WIN32)
	target_compile_definitions(bin2h PRIVATE _UNICODE) 
	target_link_options(bin2h PRIVATE /ENTRY:wmainCRTStartup )
endif()