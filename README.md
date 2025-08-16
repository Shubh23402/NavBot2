# 🧭 NavBot 2  

NavBot 2 is an **autonomous mobile robot** capable of solving maze-like environments using **SLAM (Simultaneous Localization and Mapping)** and autonomous navigation.  
The robot builds a map of its surroundings using **laser scan data**, simulated in **Gazebo**, and then plans a path to navigate itself out of the maze.  
The maze world itself is also created inside **Gazebo**, and navigation is visualized and controlled in **RViz**.

---

## ✨ Features
- 🔹 **Gazebo Simulation** – Maze world created and simulated in Gazebo.  
- 🔹 **SLAM Mapping** – Generates a 2D occupancy grid map of the maze from LIDAR data.  
- 🔹 **Autonomous Navigation** – Uses Nav2 stack to escape the maze.  
- 🔹 **ROS 2 + RViz Integration** – Real-time visualization and goal setting.  
- 🔹 **Laser Scan Sensor** – Detects obstacles and builds the map.  

---

## 🛠️ Tech Stack
- **ROS 2 (Humble)** – Middleware for robotics.  
- **Gazebo** – Physics simulator for the maze environment.  
- **RViz** – Visualization and navigation goal setting.  
- **SLAM Toolbox** – For mapping in real time.  
- **Nav2 Stack** – Path planning & autonomous navigation.  
- **LIDAR / Laser Scan** – Simulated sensor for SLAM.  

---

## 🚀 How It Works
- **Simulation in Gazebo**  
   - A custom maze world is created in **Gazebo**.  
   - The robot is spawned inside the maze with LIDAR attached.  

- **SLAM Phase**  
   - Robot explores the maze, generating a **2D occupancy grid map**.  

- **Navigation Phase**  
   - In **RViz**, the user provides a navigation goal (e.g., maze exit).  
   - Nav2 computes the path and the robot autonomously navigates out.  
