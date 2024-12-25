# Autonomous Mobile Robot Project

This repository contains the code and resources for my autonomous mobile robot project, developed and tested using the **ROS2 Foxy** framework and **Gazebo Classic** simulations. The project showcases a fully functional virtual robot capable of mapping, localization, and navigation.

---

## Features

- **Robot Description**: Modeled using **URDF** for realistic simulations in Gazebo.
- **Control Mechanisms**: 
  - Utilized **ROS2 control** for robot movement.
  - Implemented a **differential drive plugin** as an alternative.
- **Sensor Integration**:
  - Simulated sensors using URDF and plugins to communicate with the ROS2 framework.
  - Incorporated **LiDAR** for environmental perception.
- **SLAM Implementation**:
  - Deployed the **SLAM Toolbox** in **online async** mode for real-time mapping and localization.
- **Visualization**: Visualized the robot and its operations in **RViz**, included with ROS.

---

## Prerequisites

To run this project, you will need:
- **ROS2 Foxy** installed on your system ([installation guide](https://docs.ros.org/en/foxy/Installation.html)).
- **Gazebo Classic** installed ([installation guide](http://gazebosim.org/tutorials?tut=install_ubuntu)).
- A system with Ubuntu 20.04 or compatible Linux distribution.

---

## Installation

1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd <repository-name>
   ```

2. Build the ROS2 workspace:
   ```bash
   colcon build
   source install/setup.bash
   ```

3. Launch the simulation:
   ```bash
   ros2 launch <package_name> <launch_file>.launch.py
   ```

---

## How It Works

### 1. Robot Description
The robot is modeled using **URDF** for a detailed and modular design. Sensors like LiDAR are integrated via plugins, ensuring accurate simulation in Gazebo.

### 2. Control System
Movement is facilitated through **ROS2 control** with a differential drive mechanism. The **diff drive plugin** serves as an alternative for simplified control scenarios.

### 3. SLAM for Mapping and Localization
The **SLAM Toolbox** operates in **online async** mode, leveraging LiDAR data to create maps and localize the robot in real-time.

### 4. Visualization
Operations are visualized in **RViz**, allowing real-time monitoring and debugging of robot behavior.

---

## Folder Structure

```
.
├── src/                  # Source files for the robot
├── urdf/                 # URDF files for robot description
├── config/               # Configuration files for sensors and controllers
├── launch/               # Launch files for running the robot
├── maps/                 # Generated maps for localization
├── rviz/                 # RViz configuration files
└── README.md             # Project documentation (this file)
```

---

## Demonstration

### Simulation in Gazebo:
![Simulation Screenshot](path/to/screenshot.png)

### SLAM in Action:
![SLAM Screenshot](path/to/screenshot.png)

(Replace `path/to/screenshot.png` with actual paths to your images or videos.)

---

## Future Work
- Hardware implementation of the system.
- Enhancing mapping algorithms for dynamic environments.
- Incorporating additional sensors for improved environmental awareness.

---

## Contact
For any queries or collaboration opportunities, feel free to connect:
- LinkedIn: [Your LinkedIn Profile](https://linkedin.com/in/your-profile)
- Email: your.email@example.com

---

## License
This project is licensed under the [MIT License](LICENSE).
