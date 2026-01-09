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
   mkdir ~/unitree_dog_ws
   cd ~/unitree_dog_ws
   git clone git@github.com:Joajibola/Unitree-dog-ros-visualisation-with-rviz.git

2. **Build the ROS 2 package:**
    ```bash
    cd Unitree-dog-ros-visualisation-with-rviz
    colcon build --symlink-install
    source install/setup.bash
    ```

3. **Launch the rviz with the URDF**
    ```bash
    ros2 launch urdf_tutorial display.launch.py model:=$PWD/dogg_description/urdf/dogg.urdf
    ```
4. **Visualise and interact**

    Rviz will open and the unitree robot dog will load up.
    Use the joint state publisher GUI to move the revolute joints interactively 