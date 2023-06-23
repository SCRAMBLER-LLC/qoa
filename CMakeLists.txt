cmake_minimum_required(VERSION 2.8.12)
project(qoaconv C)

add_definitions(-DQOACONV_HAS_DRFLAC)

add_executable(qoaconv dr_flac.h qoaconv.c)
target_link_libraries(qoaconv PRIVATE m)
