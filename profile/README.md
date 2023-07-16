# ros-event-camera

This collection of repositories provides ROS support for event based cameras.

- [metavision_driver](https://www.github.com/ros-event-camera/metavision_driver/)
  a ROS driver for event cameras based on the MetaVision SDK
  (Prophesee)

- [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/)
  Message definitions for sending event camera data within the ROS
  framework.

- [event_camera_codecs](https://www.github.com/ros-event-camera/event_camera_codecs/)
  A C++ library to decode the events contained in
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/).

- [event_camera_py](https://www.github.com/ros-event-camera/event_camera_py/)
  Fast reading and decoding of
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/)
  in python using  pybind11 to access
  [event_camera_codecs](https://www.github.com/ros-event-camera/event_camera_codecs/)
  as a python module.  The camera events are presented as structured
  numpy arrays in the same format that the MetaVision SDK uses.

- [event_camera_viewer](https://www.github.com/ros-event-camera/event_camera_viewer/)
  Renders time slices of camera events and publishes them as images
  for viewing with tools such as ``rqt_gui``.

- [event_camera_tools](https://www.github.com/ros-event-camera/event_camera_tools/)
  Various tools to convert rosbags with legacy DVS and Prophesee messages or
  MetaVision RAW files to rosbags using
  [event_camera_msgs](https://www.github.com/ros-event-camera/event_camera_msgs/).
