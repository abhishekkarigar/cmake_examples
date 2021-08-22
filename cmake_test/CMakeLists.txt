cmake_minimum_required (VERSION 2.6)

project (cmake_test)


set ( PROJECT_LINK_LIBS libtestStudent.so )
link_directories( "/usr/lib" )

message("here")
include_directories( "/mnt/d/OCEAN_EXPLORER/C++/cmake_test/studentLibrary/include" )

add_executable( libtest cmake_test.cpp )
target_link_libraries( libtest ${PROJECT_LINK_LIBS} )


