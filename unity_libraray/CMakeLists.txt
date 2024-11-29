cmake_minimum_required(VERSION 3.8)

#make unity library
# message(STATUS "cmake - unity library")
message("cmake - unity library")

set(UNITY_LIB unity)
set(CMAKE_C_STANDARD 99)
set(CMAKE_CXX_STANDARD 14)

# project(${UNITY_LIB})

include_directories(
    unity.framework/extras/fixture/src 
    unity.framework/src/
)

# add_library(${UNITY_LIB}
#     unity.framework/src/unity.c
#     unity.framework/extras/fixture/src/unity_fixture.c
# )

add_library(${UNITY_LIB} STATIC
    unity.framework/src/unity.c
    unity.framework/extras/fixture/src/unity_fixture.c
)