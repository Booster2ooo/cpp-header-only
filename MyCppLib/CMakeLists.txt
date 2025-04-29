# CMakeList.txt : CMake project for MyCppLib, include source and define
# project specific logic here.
#

# Add source to this project's library.
add_library(MyCppLib INTERFACE)
target_include_directories(MyCppLib INTERFACE ${CMAKE_CURRENT_SOURCE_DIR})
target_compile_features(MyCppLib INTERFACE cxx_std_20)
# TODO: Add tests and install targets if needed.
