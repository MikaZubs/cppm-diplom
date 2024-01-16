cmake_minimum_required(VERSION 3.18.0)
project(TS VERSION 1.0)
set(SOURCE_DLL vehicle.h vehicle.cpp AirTs.h AirTs.cpp eagle.h eagle.cpp carpet.h carpet.cpp broom.h broom.cpp GndTs.h GndTs.cpp boots.h boots.cpp camel.h camel.cpp camelracer.h camelracer.cpp centaur.h centaur.cpp)
add_library(${PROJECT_NAME} SHARED ${SOURCE_DLL})