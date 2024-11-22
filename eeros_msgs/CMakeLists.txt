cmake_minimum_required(VERSION 3.8)
project(eeros_msgs)

# find dependencies
find_package(ament_cmake REQUIRED)
find_package(builtin_interfaces REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME}
  "msg/AnalogSignal.msg"
  "msg/DigitalSignal.msg"
  DEPENDENCIES builtin_interfaces
)

ament_package()
