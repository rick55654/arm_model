cmake_minimum_required(VERSION 3.5)
project(arm_model)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY launch learm_meshes xarm_meshes rviz urdf
  DESTINATION share/${PROJECT_NAME}
)

ament_export_dependencies(${THIS_PACKAGE_INCLUDE_DEPENDS})

ament_package()
