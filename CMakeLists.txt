# voir exemple:
#   https://github.com/vgonisanz/cmake-pandocology-sample/blob/master/CMakeLists.txt

cmake_minimum_required(VERSION 3.0)


SET(PROJ_MAIN_NAME "techNotes")
PROJECT(${PROJ_MAIN_NAME}-main NONE)

LIST(APPEND CMAKE_MODULE_PATH "${CMAKE_SOURCE_DIR}/cmake/cmake-pandocology")
INCLUDE(pandocology)
INCLUDE(cmspandoc)


CONFIGUREPANDOCOLOGY()
SET(${PROJ_MAIN_NAME}_PATH_MAIN ${CMAKE_SOURCE_DIR} CACHE PATH "This directory contains initial Path" )


Add_subdirectory(src/git)
