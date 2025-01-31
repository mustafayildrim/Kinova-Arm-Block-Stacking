# Kinova Arm Block Stacking Project

## Description

This project involves programming a **Kinova robotic arm** to pick up a block positioned **20 cm in front of the robot**, aligned with the **(x, y) coordinate frame** of the arm. The arm will then transport the block to a designated **(x, y, z) location** and release it. The process is repeated to build a **three-block-high stack** at a specified location.

## Features

- **Block Pickup:** The Kinova arm grabs a block at a fixed starting position.
- **Block Transport:** Moves the block to a designated **(x, y, z) coordinate**.
- **Block Release:** Places the block at the target location.
- **Stacking Mechanism:** Repeats the process to form a **three-block-high** stack.

## Technologies Used

- **Python**
- **Kinova Kortex API**
- **ROS (Robot Operating System)**



## Installation

```bash
pip install kinova-ros scipy numpy
```

## Project Tasks

### **Task 1: Initialize and Calibrate the Kinova Arm**

- Establish a connection using **Kinova Kortex API**.
- Move the arm to a **home/safe position** before operations.

### **Task 2: Block Pickup**

- Move the arm to the **pre-grasp position** using angular motion.
- Use the gripper (`set_gripper(base, position)`) to grab the block.

### **Task 3: Block Transport and Placement**

- Execute **joint angle movements** (`example_angular_action_movement()`) to lift the block.
- Open the gripper to **release the block**.

### **Task 4: Stack Three Blocks**

- Repeat the pickup and placement sequence three times.
- Adjust the final placement height to form a stack of three blocks.

## Visualizations

- **Trajectory Visualization:** Plot planned motion paths.
- **Final Stacked Structure:** Display the completed stack.



