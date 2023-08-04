# ros-event-camera

This collection of repositories provides ROS support for event based cameras.

## Repositories/Packages

- [metavision_driver](https://www.github.com/ros-event-camera/metavision_driver/):
  a ROS driver for event cameras based on the MetaVision SDK (Prophesee).
  Build status: [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__metavision_driver__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__metavision_driver__ubuntu_jammy_amd64/) [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__metavision_driver__ubuntu_jammy_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__metavision_driver__ubuntu_jammy_amd64/)

- [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/):
  message definitions for sending event camera data within the ROS
  framework.

- [event_camera_codecs](https://www.github.com/ros-event-camera/event_camera_codecs/):
  a C++ library to decode the events contained in
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/).

- [event_camera_py](https://www.github.com/ros-event-camera/event_camera_py/):
  fast reading and decoding of
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/)
  in python using  pybind11 to access
  [event_camera_codecs](https://www.github.com/ros-event-camera/event_camera_codecs/)
  as a python module.  The camera events are presented as structured
  numpy arrays in the same format that the MetaVision SDK uses.

- [event_camera_viewer](https://www.github.com/ros-event-camera/event_camera_viewer/):
  renders time slices of camera events and publishes them as images
  for viewing with tools such as rqt_gui.

- [event_camera_tools](https://www.github.com/ros-event-camera/event_camera_tools/):
  various tools to:
   - convert rosbags with legacy DVS and Prophesee messages or  MetaVision RAW files to rosbags using
    [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/).
   - echo decoded event messages
   - display event rate and measure messaging performance
   - check synchronization between cameras

## How to manage and release repositories

[Here are more instructions](docs/manage_repositories.md) on how to manage and release the ros-event-camera repositories.



