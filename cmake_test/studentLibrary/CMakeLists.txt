cmake_minimum_required (VERSION 2.6)

project (studentLibrary_test)
set(CMAKE_BUILD_TYPE Release)

#Bring the headers ,.h files into the project
include_directories(include)

file(GLOB SOURCES "src/*.cpp")

add_library(testStudent SHARED ${SOURCES})

#add_executable(cmake_test ${SOURCES})

install(TARGETS testStudent DESTINATION /usr/lib)
