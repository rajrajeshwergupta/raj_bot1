# Autonomous Mobile Robot Project  

This repository contains the code for an **Autonomous Mobile Robot** developed and tested using **ROS2 Humble** and **Gazebo Ignition Fortress**. The project focuses on creating a robot capable of **mapping, localization, path planning, and autonomous navigation** in a simulated environment.  

## Features  
- **Robot Description**: Modeled using **URDF** for simulation in Gazebo.  
- **Control System**: Implemented with **ROS2 control** and a **differential drive plugin** for movement.  
- **SLAM**: Integrated **SLAM Toolbox** with **LiDAR sensor** in **online async mode** for real-time mapping and localization.  
- **Path Planning & Navigation**: Implemented the **Nav2 stack** for autonomous path planning.  
- **Visualization**: Used **RViz** for monitoring robot performance and map generation.  

## Repository Structure  
- `src/`: ROS2 package source files.  
- `description/`: Robot description files in URDF format.  
- `config/`: Configuration files for SLAM Toolbox and Nav2.  
- `launch/`: ROS2 launch files for simulations and navigation.  
