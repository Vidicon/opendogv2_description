cmake_minimum_required(VERSION 3.0.2)
project(opendogv2_description)

find_package(catkin
  REQUIRED COMPONENTS
    roslaunch
)

catkin_package(
  CATKIN_DEPENDS
)

# Install directories
install(
  DIRECTORY
    config
    launch
    urdf
  DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION})
