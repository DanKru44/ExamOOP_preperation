cmake_minimum_required( VERSION 3.10 )
project( HelloWorld )
message( "Hello World" )

add_library( hello STATIC hello.cpp )
add_executable( ${PROJECT_NAME} main.cpp )
target_link_libraries( ${PROJECT_NAME} hello )
