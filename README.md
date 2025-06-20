# Autonomous House-Organizing Robot (ROS2)

This repository presents the autonomous navigation module developed for a simulated house-organizing robot using **ROS2**, **Nav2**, and **Gazebo**. The robot was designed to operate in an unknown indoor environment, explore the space, and perform basic organization tasks.

> 🧾 This module is part of a larger project from **MIE1075: Autonomous Systems Engineering**, University of Toronto.  
> 🛠️ Repo focuses on **navigation logic only**. Manipulation and system integration were handled separately.


## 🚧 Project Overview

The robot simulates an autonomous assistant deployed in a residential environment. Its goals include:

- Navigating an unfamiliar map
- Exploring rooms and locating target objects
- Maneuvering around dynamic and static obstacles


## 🧠 Key Features

- **Frontier-Based Exploration**  
  Used to identify navigable unknown regions of the map for efficient coverage.

- **Goal-Directed Planning with A\***  
  Implemented traditional A\* path planning for initial exploration and movement toward frontier targets.

- **Mapless Navigation with DDPG**  
  Integrated a pretrained Deep Deterministic Policy Gradient (DDPG) policy to reach targets in constrained or partially occluded environments where classical planning fails.

- **Scenario-Specific Behaviors**  
  Designed multiple strategies for three distinct exploration cases:  
  1. Open exploration  
  2. Navigating dark (unknown) spaces  
  3. Navigating occluded corners using mapless RL control

## 🚧 Code Availability
The codebase is currently being cleaned and will be uploaded shortly.

## 📹 Demo



https://github.com/user-attachments/assets/a2527b5e-307a-40a5-80d7-0f8de7f0c4a0



> The robot incrementally builds a map of the unknown environment and navigates to unexplored frontiers using A\* path planning.


---

## 🔍 Future Work

- Integration with object recognition and manipulation modules  
- Real-time coordination between classical and RL-based navigation policies  
- Deployment to physical robots
