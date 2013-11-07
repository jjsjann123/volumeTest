cmake_minimum_required(VERSION 2.8.1)
project(myvolume)

find_package(Omegalib)

include_directories(${OMEGA_INCLUDE_DIRS})        
add_executable(myvolume osgvolume.cpp)
target_link_libraries(myvolume ${OMEGA_LIB} ${OMEGA_TOOLKIT_LIB} ${OMEGA_OSG_LIB})

