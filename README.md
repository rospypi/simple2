# **THIS IS NOT THE OFFICIAL ROS2 INDEX SERVER**

# Python index server for ROS2

## What is this for?

This is Python index server for ROS2(https://rospypi.github.io/simple2/).
Not only Python packages(ex. rclpy) but also tools(ex. rviz2) and libraries(ex. rcl) can be installed into the virtual env.

Supported Python versions: 3.6, 3.7, 3.8

Support platforms: Linux, MacOSX

(Not all packages are tested.)

## How to use

```bash
virtualenv -p python3 venv
. ./venv/bin/activate
pip install --extra-index-url https://rospypi.github.io/simple/ rclpy rviz2 ros2py-init
ros2py-init; deactivate; . ./venv/bin/activate  # this is needed only once
rviz2
```

## Development

All the packages are build by [this repository](https://github.com/otamachan/ros2py).
