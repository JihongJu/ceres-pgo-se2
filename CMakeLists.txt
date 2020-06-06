# cmake version to be used
cmake_minimum_required( VERSION 3.0 )

# project name
project(ceres_pgo)

# target
add_executable( helloworld helloworld.cpp )

# external libs
find_package(Ceres REQUIRED)

target_include_directories(helloworld
  PRIVATE
    ${CERES_INCLUDE_DIRS}
)

target_link_libraries(helloworld
  PRIVATE
    ${CERES_LIBRARIES}
)
