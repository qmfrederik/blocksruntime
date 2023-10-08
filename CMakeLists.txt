cmake_minimum_required(VERSION 3.9)

project(BlocksRuntime)

add_library(
    BlocksRuntime
    data.c
    runtime.c)

set_target_properties(
    BlocksRuntime
    PROPERTIES
    PUBLIC_HEADER
    "Block.h;Block_private.h")

install(
    TARGETS BlocksRuntime)