# cmake version to be used
cmake_minimum_required( VERSION 3.0 )

# project name
project(ceres_pgo)

include_directories( ./include)

# target
add_executable(pose_graph_2d ./src/pose_graph_2d.cpp)

# external libs
find_package(Ceres REQUIRED)

target_include_directories(pose_graph_2d
  PRIVATE
    ${CERES_INCLUDE_DIRS}
)

target_link_libraries(pose_graph_2d
  PRIVATE
    ${CERES_LIBRARIES}
)
