CMAKE_MINIMUM_REQUIRED( VERSION 3.1 )

PROJECT( LIBRARIES )

set( CMAKE_MODULE_PATH ${CMAKE_SOURCE_DIR}/cmake ${CMAKE_SOURCE_DIR}/../cmake ${CMAKE_MODULE_PATH} )

INCLUDE( SetupC++11 )

INCLUDE( ExternalProject )

INCLUDE( External_STEPCode )

# Set targeted variables in file to be read by CMake
configure_file(
   ${CMAKE_SOURCE_DIR}/cmake/Libraries_Config.cmake.in
   ${CMAKE_BINARY_DIR}/Libraries_Config.cmake
   @ONLY
)
