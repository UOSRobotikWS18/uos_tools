# Catkin User Guide: http://www.ros.org/doc/groovy/api/catkin/html/user_guide/user_guide.html
# Catkin CMake Standard: http://www.ros.org/doc/groovy/api/catkin/html/user_guide/standards.html
cmake_minimum_required(VERSION 2.8.3)
project(uos_gazebo_worlds)
# Load catkin and all dependencies required for this package
find_package(catkin REQUIRED)

catkin_package()

install(DIRECTORY
    launch/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch
)

install(DIRECTORY
    Media/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/Media
)

install(DIRECTORY
    worlds/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/worlds
)
