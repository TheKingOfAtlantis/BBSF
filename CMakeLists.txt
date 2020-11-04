cmake_minimum_required(VERSION 3.17.0)
project(BBSF
    DESCRIPTION "Binary Biological Sequences Format"
    VERSION 0.0.1
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)


add_library(libBBSF STATIC "")
set_target_properties(libBBSF PROPERTIES LINKER_LANGUAGE CXX)
target_sources(libBBSF PUBLIC
    "src/BBSF.cppm"
)
