# 🧭 NavBot 

NavBot is an **autonomous mobile robot** capable of solving maze-like environments and navigating real-world layouts using **SLAM (Simultaneous Localization and Mapping)** and the **ROS 2 Navigation Stack**.  
The robot builds a map of its surroundings using **laser scan data** in **Gazebo simulation** and then autonomously navigates to a user-defined goal location in **RViz**.  

In addition to maze-solving, NavBot 2 has also been extended to a **real-world use case**:  
🏠 Using a custom **Gazebo layout of my hostel floor**, the robot generates a map using SLAM and can autonomously navigate to different **rooms and corridors** as required.  

---

## ✨ Features
- 🔹 **Gazebo Simulation** – Maze world and custom hostel floor layout created and simulated in Gazebo.  
- 🔹 **SLAM Mapping** – Generates a 2D occupancy grid map of unknown environments.  
- 🔹 **Autonomous Navigation** – Uses the Nav2 stack to plan and execute paths.  
- 🔹 **Room Navigation** – Can navigate to specific rooms in the hostel floor map.  
- 🔹 **ROS 2 + RViz Integration** – Provides real-time visualization, goal setting, and monitoring.  
- 🔹 **Laser Scan Sensor** – Simulated LIDAR used for mapping and obstacle detection.  

---

## 🛠️ Tech Stack
- **ROS 2 (Humble)** – Middleware for robotics.  
- **Gazebo** – Physics simulator for maze and hostel layout environments.  
- **RViz** – Visualization and navigation goal setting.  
- **SLAM Toolbox** – For map generation in real time.  
- **Nav2 Stack** – Path planning and autonomous navigation.  
- **LIDAR / Laser Scan** – Simulated sensor input for SLAM and navigation.  

---

## 🚀 How It Works
- **Simulation in Gazebo**  
   - A **maze world** and a **hostel floor layout** are created in **Gazebo**.  
   - The robot is spawned inside the environment with a LIDAR sensor attached.  

- **SLAM Phase**  
   - Robot explores the environment to generate a **2D occupancy grid map**.  
   - Works for both **maze navigation** and **hostel floor mapping**.  

- **Navigation Phase**  
   - In **RViz**, the user sets a navigation goal (maze exit or specific room).  
   - Nav2 computes the optimal path and the robot navigates autonomously to the destination.  

---
