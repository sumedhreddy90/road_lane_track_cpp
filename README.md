# road_lane_track_cpp

System Dependencies

    Ubuntu 20.04.2 LTS
    ROS Noetic
    cmake = 3.16.3
    OpenCV >= 3.4.2
    

Launch Steps

1. Go to ~/catkin_ws and run catkin_make

2. Edit /launch/lane_detection.launch file to select the video file of your input, under the param video_filename

3. Run the launch file roslaunch lane_detection lane_detection.launch


There's two nodes inside this package:

    1. video-parser

    This node takes in an input video access that is connected to your computer and convert it to sensor_msgs::Image ROS topic

    2. lane-detector

    This node takes an input sensor_msgs::Image topic and output another sensor_msgs::Image topic with the lane lines overlaid on the original image


    
file:///home/sumedh/Pictures/Screenshot%20from%202021-06-10%2014-30-39.png![image](https://user-images.githubusercontent.com/24978535/121496993-9d1e1980-c9f8-11eb-9400-d0e9f6a59090.png)

