# hikcam_xsens_platform
Hikrobot camera + XSens IMU platform.

## Xsens IMU Usage
Install dependencies from: [http://wiki.ros.org/xsens_mti_driver](http://wiki.ros.org/xsens_mti_driver)  
And then compile.

Usage
- Modify the config file: usb-X, and buadrate, in `xsens_ros_mti_driver/param/xsens_mti_node.yaml`
- 
```bash
# Change USB's latency level.
sudo sh -c 'echo 1 > /sys/bus/usb-serial/devices/ttyUSB0/latency_timer'
# usb's mothod
sudo chmod  777 /dev/ttyUSB0

# Run IMU with display
roslaunch xsens_mti_driver display.launch

# Run pure IMU
roslaunch xsens_mti_driver xsens_mti_node.launch
```


## Hikrobot camera
Check [this](https://github.com/LarryDong/HIKROBOT-MVS-CAMERA-ROS)

