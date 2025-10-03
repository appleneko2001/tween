# actually, who cares cmake_mininum_required() ?
# newest cmake have already removing backward standard support
project(tween)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++0x")

add_library(tween
        callback.h
        tween.cpp
        tween.h
)

target_include_directories(
        tween INTERFACE
        $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}>
        $<INSTALL_INTERFACE:${CMAKE_INSTALL_INCLUDEDIR}>
)