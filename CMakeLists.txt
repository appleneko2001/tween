# actually, who cares cmake_mininum_required() ?
# newest cmake have already removing backward standard support
project(tween)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++0x")

add_library(tween
        callback.h
        tween.cpp
        tween.h
)