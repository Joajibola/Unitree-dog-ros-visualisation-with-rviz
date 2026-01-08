# Unitree Dog ROS 2 Visualisation with RViz

This repository provides a ROS 2 workspace for the kinematic visualization of a Unitree quadruped robot (Go Dog) using URDF and RViz2. It allows users to explore the robot's structure and interact with joint movements via the RVIZ GUI.



## 🚀 Features
* **High-Fidelity Meshes:** Includes `.dae` files for the trunk, hip, thigh, and calf.
* **Complete Kinematic Tree:** Properly defined joints and links for a quadruped.
* **Interactive Control:** Integrated with `joint_state_publisher_gui` for real-time joint manipulation.

## 🛠️ Prerequisites
* **ROS 2 Version:** Jazzy (Works with Humble/Foxy as well)
* **Packages:** * `urdf_tutorial`
  * `robot_state_publisher`
  * `joint_state_publisher_gui`
  * `rviz2`

## 📦 Installation & Build

1. **Clone the repository:**
   ```bash
   mkdir -p ~/unitree_dog_ws/src
   cd ~/unitree_dog_ws/src
   git clone [https://github.com/Joajibola/Unitree-dog-ros-visualisation-with-rviz.git](https://github.com/Joajibola/Unitree-dog-ros-visualisation-with-rviz.git) .
