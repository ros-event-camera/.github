# ros-event-camera

This collection of repositories provides ROS support for event based cameras.

## Repositories/Packages

- [metavision_driver](https://www.github.com/ros-event-camera/metavision_driver/):
  a ROS driver for event cameras based on the MetaVision SDK (Prophesee).\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__metavision_driver__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__metavision_driver__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__metavision_driver__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__metavision_driver__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__metavision_driver__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__metavision_driver__ubuntu_noble_amd64/)

- [libcaer_driver](https://www.github.com/ros-event-camera/libcaer_driver/):
  a ROS2 driver for event cameras based on Inivation Lab's CAER library (Davis, DvXplorer).\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__libcaer_driver__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__libcaer_driver__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__libcaer_driver__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__libcaer_driver__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__libcaer_driver__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__libcaer_driver__ubuntu_noble_amd64/)

- [libcaer](https://www.github.com/ros-event-camera/libcaer/):
  a ROS2 package wrapped around Inivation Lab's CAER library (Davis, DvXplorer).\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__libcaer__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__libcaer__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__libcaer__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__libcaer__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__libcaer__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__libcaer__ubuntu_noble_amd64/)
  
- [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/):
  message definitions for sending event camera data within the ROS framework.\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__event_camera_msgs__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__event_camera_msgs__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__event_camera_msgs__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__event_camera_msgs__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__event_camera_msgs__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__event_camera_msgs__ubuntu_noble_amd64/)

- [event_camera_codecs](https://www.github.com/ros-event-camera/event_camera_codecs/):
  a C++ library to decode the events contained in
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/).\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__event_camera_codecs__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__event_camera_codecs__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__event_camera_codecs__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__event_camera_codecs__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__event_camera_codecs__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__event_camera_codecs__ubuntu_noble_amd64/)

- [event_camera_py](https://www.github.com/ros-event-camera/event_camera_py/):
  fast reading and decoding of
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/)
  in python using  pybind11 to access
  [event_camera_codecs](https://www.github.com/ros-event-camera/event_camera_codecs/)
  as a python module.  The camera events are presented as structured
  numpy arrays in the same format that the MetaVision SDK uses.\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__event_camera_py__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__event_camera_py__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__event_camera_py__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__event_camera_py__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__event_camera_py__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__event_camera_py__ubuntu_noble_amd64/)

- [event_camera_renderer](https://www.github.com/ros-event-camera/event_camera_renderer/):
  renders time slices of camera events and publishes them as images
  for viewing with tools such as rqt_gui.\
  Build status:
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Hdev__event_camera_renderer__ubuntu_jammy_amd64&subject=Humble)](https://build.ros2.org/job/Hdev__event_camera_renderer__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Idev__event_camera_renderer__ubuntu_jammy_amd64&subject=Iron)](https://build.ros2.org/job/Idev__event_camera_renderer__ubuntu_jammy_amd64/)
  [![Build Status](https://build.ros2.org/buildStatus/icon?job=Rdev__event_camera_renderer__ubuntu_noble_amd64&subject=Rolling)](https://build.ros2.org/job/Rdev__event_camera_renderer__ubuntu_noble_amd64/)

- [event_camera_tools](https://www.github.com/ros-event-camera/event_camera_tools/):
  various tools to:
   - convert rosbags with legacy DVS and Prophesee messages or  MetaVision RAW files to rosbags using
    [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/).
   - echo decoded event messages
   - display event rate and measure messaging performance
   - check synchronization between cameras

## How to manage and release repositories

[Here are more instructions](docs/manage_repositories.md) on how to manage and release the ros-event-camera repositories.



