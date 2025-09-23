cmake_minimum_required (VERSION 3.28)
project (OtaryxDemo)

add_executable (otaryx_demo main.cpp)

install (TARGETS otaryx_demo DESTINATION /usr/bin)
