cmake_minimum_required(VERSION 3.5)
project(atl_launch)

find_package(ament_cmake REQUIRED)
# find_package(learning_tf2_cpp)

install(DIRECTORY launch
  DESTINATION share/${PROJECT_NAME})

if(BUILD_TESTING)
  find_package(ament_lint_auto REQUIRED)
  set(ament_cmake_copyright_FOUND TRUE)
  ament_lint_auto_find_test_dependencies()

 
endif()

ament_package()
