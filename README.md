🚦 Traffic Light Detection in Duckietown 2024

Welcome to the repository for the Traffic Light Detection in Duckietown 2024 project! This system provides Duckiebots with the ability to detect and respond to traffic lights and red lines autonomously. The project leverages ROS (Robot Operating System), computer vision, and deep learning techniques to enhance autonomous behavior in Duckietown environments.

📚 Project Overview

The goal of this project is to equip Duckiebots with:

Traffic Light Detection: Identify traffic lights and determine if they are red or green using a YOLO Nano deep learning model.
State Machine Integration: Manage Duckiebot behavior such as stopping and proceeding based on traffic light signals.
Red Line Detection: Recognize red lines on the road to make informed decisions about stopping at intersections.
This system allows the Duckiebot to interact with traffic infrastructure in a controlled environment, enabling autonomous navigation and compliance with traffic rules.

🚀 How to Run the Project

Prerequisites
Docker with Duckietown images installed.
ROS Noetic.
Catkin Workspace set up.
Step-by-Step Instructions
Build the Project:
cd ~/catkin_ws
catkin build state_machine_pkg
source devel/setup.bash
Run the Traffic Light Detection Node:
rosrun state_machine_pkg runner.py
Run the State Machine Node:
rosrun state_machine_pkg state_machine_node.py
Run the Red Line Detection Node (Optional):
rosrun state_machine_pkg red_line_detection_node.py


🛠️ Dependencies

Ensure the following dependencies are installed:

ROS Noetic (Ubuntu 20.04)
OpenCV (cv2)
NumPy
Torch (for traffic light detection)
Docker
🤝 Contributors

This project is developed by the Duckie-Dynamics team:

🧑‍💻 Himanshu Joshi
👩‍💻 Bingjie Xue
🧑‍💻 Angel Manzano
🧑‍💻 Thorbjörn Höllwarth
