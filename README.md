# ROS 2 Autonomous Mobile Manipulator

This project implements a fully integrated autonomous robot system using **ROS 2 Humble**. It features a 3-DOF robotic arm mounted on a differential drive mobile base, capable of vision-guided grasping and multi-modal interaction.

## 🚀 Key Features
- **Autonomous Navigation**: Integrated with `Nav2` and `SLAM Toolbox` for environment mapping and path planning.
- **Vision-based Grasping**: Real-time object detection using `OpenCV` and motion planning via `MoveIt 2`.
- **Multi-modal HRI**: 
  - **Gesture Control**: Hand tracking and command triggering using `Google MediaPipe`.
  - **Voice Recognition**: Offline Chinese voice command processing using `Vosk`.
- **Custom Simulation**: Built-in Gazebo world with optimized physics parameters.

## 🛠 Tech Stack
- **Languages**: C++, Python
- **Middleware**: ROS 2 Humble
- **Tools**: Gazebo 11, MoveIt 2, Nav2, MediaPipe, Vosk, SolidWorks

## 📺 Demo
*(Here you can upload a GIF or a link to a video demonstrating the car moving and grasping)*

## 🏃 How to Run
1. Start Simulation:
   `ros2 launch car_model_moveit_config demo_gazebo.launch.py`
2. Start Navigation:
   `ros2 launch car_model navigation.launch.py`
3. Start Mission Control:
   `ros2 launch car_model gesture_mission.launch.py`
