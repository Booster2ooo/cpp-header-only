# CMakeList.txt : CMake project for MyCppApp, include source and define
# project specific logic here.
#
# Get all .cpp and .h files in this directory
file(GLOB APP_SOURCES "*.cpp" "*.h")

# Add source to this project's executable.
add_executable (MyCppApp ${APP_SOURCES})

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET MyCppApp PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
target_link_libraries(MyCppApp PRIVATE MyCppLib)