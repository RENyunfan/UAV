# px4

## 1 安装

https://blog.csdn.net/weixin_43568893/article/details/104533500

## 2 Gazebo仿真编译报错

```bash
GSTREAMER_LIBRARIES (ADVANCED)
    linked by target "LiftDragPlugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_gst_camera_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_barometer_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_geotagged_images_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_magnetometer_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "sensor_msgs" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_irlock_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_video_stream_widget" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_controller_interface" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_wind_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "std_msgs" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_gps_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_sonar_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "mav_msgs" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "nav_msgs" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_lidar_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_opticalflow_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_mavlink_interface" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_uuv_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_vision_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_multirotor_base_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_imu_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_gimbal_controller_plugin" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "physics_msgs" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo
    linked by target "gazebo_motor_model" in directory /home/sch/catkin_ws/src/Firmware/Tools/sitl_gazebo

-- Configuring incomplete, errors occurred!

```

### 原因是缺少依赖

```bash
sudo apt-get install libgstreamer-plugins-base1.0-dev
```

