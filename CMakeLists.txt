cmake_minimum_required(VERSION 3.19)
project(gdextension-gameplay)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_POSITION_INDEPENDENT_CODE ON)

include(FetchContent)

FetchContent_Declare(
	GDExtension
	GIT_REPOSITORY https://github.com/godotengine/godot-cpp.git
	GIT_TAG godot-4.0-stable
)

FetchContent_MakeAvailable(GDExtension)

add_subdirectory(gameplay)
