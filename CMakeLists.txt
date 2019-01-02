cmake_minimum_required(VERSION 2.8.4)

set(SOURCE_DIR "/home/wataru/CLionProjects/LKH-2.0.9")
set(PROJECT_BINARY_DIR  "/home/wataru/CLionProjects/LKH-2.0.9")

set(IDIR "INCLUDE")
set(TREE_TYPE "TWO_LEVEL_TREE")
set(CMAKE_C_FLAGS "-O0 -Wall -I${IDIR} -D${TREE_TYPE} -g" )

# set project name
project(LKH)

add_custom_target(LKH COMMAND make -C ${SOURCE_DIR} CLION_EXE_DIR=${PROJECT_BINARY_DIR})