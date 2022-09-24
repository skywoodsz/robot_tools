cmake_minimum_required(VERSION 3.0.2)
project(ompl_learn)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# release
# SET(CMAKE_BUILD_TYPE "Release")

find_package(catkin REQUIRED COMPONENTS
  roscpp
  std_msgs
)

find_package(Eigen3 REQUIRED)
set(Eigen3_INCLUDE_DIRS ${EIGEN3_INCLUDE_DIR})

catkin_package(
 INCLUDE_DIRS include
)

###########
## Build ##
###########

include_directories(
  include
  ${catkin_INCLUDE_DIRS}
  ${Eigen3_INCLUDE_DIRS}
)

# add_library(
#         )
# target_link_libraries(
#         ${catkin_LIBRARIES}
#         )


###########
##  EXE  ##
###########

add_executable( 
        )

target_link_libraries(
        ${catkin_LIBRARIES}
        )

