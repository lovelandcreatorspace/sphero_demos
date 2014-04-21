cmake_minimum_required(VERSION 2.8.3)
project(sphero_demos)

find_package(catkin REQUIRED COMPONENTS)

catkin_package()
catkin_python_setup()

install(
  PROGRAMS 
    scripts/sphero_color_demo
    scripts/sphero_collision_demo
    scripts/sphero_teleop_demo
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)
