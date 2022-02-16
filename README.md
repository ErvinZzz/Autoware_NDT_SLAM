# Autoware_NDT_SLAM
Transplant NDT_SLAM Package by YamatoAndo in Autoware.AI 1.12.0 https://github.com/YamatoAndo/autoware/tree/feature/ndt_slam_for_pr/ros/src/computing/perception/localization/packages/lidar_localizer/nodes/ndt_slam

## Getting Started

### Dependencies

* Ubuntu 18.04, ROS melodic
* Cuda 10.2
* Eigen >= 3.3.7

### Installing

```
cd Autoware_NDT_SLAM
rosdep update
rosdep install -y --from-paths src --ignore-src --rosdistro $ROS_DISTRO
AUTOWARE_COMPILE_WITH_CUDA=1 colcon build --cmake-args -DCMAKE_BUILD_TYPE=Release
```

## Todo
* Add loop closure detection on backend
* Node generating Real-time vector map for in-door navigatio
