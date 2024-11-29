cmake_minimum_required(VERSION 3.8)

set(PROJECT unity_top_project)

project(${PROJECT})

message("Project top : ${PROJECT}")

# add_subdirectory(src)
# add_subdirectory(test)
add_subdirectory(unity.lib)

