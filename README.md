# **RT2 Assignment** 
This repository contains three directories each of them relates to the corresponding assingment, is introduced in the following way:
# 1- docs directory

## Research Track 2 Documentation
The directory contains information and documentation related to the Research Track 1_second assignment.

The address is: [https://ehsan51.github.io/RT2_assignment/](https://ehsan51.github.io/RT2_assignment/)

The environment of this address is as following:

![image](https://github.com/ehsan51/RT2_assignment/assets/52650110/ae122c91-e37c-4e33-9063-df2792e08808)


### Table of Contents
- [Indices and Tables](#indices-and-tables)
- [Robot_Controller Documentation](#robot-controller-documentation)
- [Firstnode Module](#module-scriptsfirstnode)
- [Secondnode Module](#module-scriptssecondnode)
- [Thirdnode Module](#module-scriptsthirdnode)
- [Fourthnode Module](#module-scriptsfourthnode)

### Indices and Tables
- [Index](genindex.html)
- [Module Index](py-modindex.html)
- [Search Page](search.html)

### Robot_Controller Documentation
This section provides documentation for the Robot_Controller package.

### Firstnode Module
The Firstnode module implements a controller for a robot using the ROS framework. It provides the following functions:
- `cancel_target()`: Sends a cancel command to the action server, canceling the current planning goal.
- `interface_space()`: Displays a controlling panel with a welcome message and a list of options for the user to select from.
- `target_client()`: Allows the user to enter the position of the robot's target and sends it to the action server.

For more details and source code, please refer to the [Firstnode Module](#module-scriptsfirstnode) documentation.

### Secondnode Module
The Secondnode module is a ROS node that receives Odometry messages from the `/odom` topic, extracts position and linear velocity data, and publishes them as custom messages of type `custom_msg` to the `chatter` topic.

For more details and source code, please refer to the [Secondnode Module](#module-scriptssecondnode) documentation.

### Thirdnode Module
The Thirdnode module is responsible for tracking the number of times a robot reaches a goal and the number of times a goal is canceled.

For more details and source code, please refer to the [Thirdnode Module](#module-scriptsthirdnode) documentation.

### Fourthnode Module
The Fourthnode module is responsible for subscribing to the `custom_msg` messages published by the Secondnode module and performing further processing or actions.

For more details and source code, please refer to the [Fourthnode Module](#module-scriptsfourthnode) documentation.

# 2- Second directory
## Robot Goal Planning and Visualization
This directory contains code to satisfy some features such as
-  Some buttons for handling the motion of the robot
-  A plot with the robot’s position and targets’ positions
-  A text box with the distance of the closest obstacle
-  A plot for the number of reached/not-reached targets

The system allows users in Jupyter Notebook to input goal positions, send goals to the robot, visualize the robot's targrt on a plot and the robot position, monitor the closest obstacle distance detected by the robot and plot the numer of reached/not-reached targets.

### Prerequisites

- ROS 
- Python 3
- IPython Widgets
- matplotlib
- actionlib
- assignment_2_2022 package
- sensor_msgs package
- nav_msgs package
- std_srvs package

### Usage

1. Clone the repository and navigate to the project directory.
     https://github.com/CarmineD8/assignment_2_2022 
3. Launch the ROS environment.
4. Launch the Jupyter Notebook.
     ``` jupyter notebook```
5. Run the following command to execute the goal planning and visualization system:
     ```roslaunch assignment_2_2022 assignment1.launch ```
6. Use the input fields to enter the X and Y positions for the robot's goal.
7. Click the "Send Goal" button to send the goal to the robot.
8. Click the "Cancel Goal" button to cancel the active goal.
9. The plot will display the robot's positions in real-time
10. The plot will display the robot's goal positions in real-time.
11. The "Closest Obstacle Distance" value will be updated based on the laser scan data received by the robot.
12. The numer of reached or canceled target will be ploted on the screen.

Here is the environment
<br> <!--  -->
 1- Gazebo
 
![image](https://github.com/ehsan51/RT2_assignment/assets/52650110/bef36a36-0347-48c8-8f69-d267caf45c83)

2-  Some buttons for handling the motion of the robot: 
<br> <!-- Some buttons for handling the motion of the robot -->
![image](https://github.com/ehsan51/RT2_assignment/assets/52650110/3697612a-1e88-4f6e-93e3-e651e9866bb7)
<br> <!-- A plot with the robot’s position and targets’ positions  -->
3- A plot with the robot’s position and targets’ positions:
<br> <!--  -->
![image](https://github.com/ehsan51/RT2_assignment/assets/52650110/97d1b45e-74e2-4e21-bba1-6f831d5455da)
<br> <!-- A text box with the distance of the closest obstacle -->
4-  A text box with the distance of the closest obstacle:
<br> <!--  -->
![image](https://github.com/ehsan51/RT2_assignment/assets/52650110/f15cb505-438b-448b-91d1-c3517138ab1e)
<br> <!--  -->
<br> <!--  A plot for the number of reached/not-reached targets: -->
5-  A plot for the number of reached/not-reached targets:

![image](https://github.com/ehsan51/RT2_assignment/assets/52650110/ce3ec1c7-3cf2-45e5-a597-05964f53cd7f)
<br> <!--  -->
# 3- Third directory
## Statistical Analysis Report

This directory contains a statistical analysis report comparing the time efficiency and success/failure rates between two approaches: "Amir" and "Mine". The report presents the experimental design, hypothesis testing, calculations, and results for both factors.

### Abstract

The abstract provides a summary of the report, highlighting the purpose of the analysis and the main findings. It mentions the significance level used for hypothesis testing.

### Introduction

The introduction section introduces the context and objectives of the report. It explains the goal of evaluating and comparing the time efficiency and success/failure rates between the "Amir" and "Mine" approaches.

### Experimental Design

The experimental design section outlines the parameters of the experiment, including the map configurations, numbers of tokens, and the number of tests conducted. It provides essential information about the data collection process.

### Time Efficiency Analysis

This section presents the analysis of time efficiency for both the "Amir" and "Mine" approaches. It includes the statistical parameters, such as sample sizes, means, and standard deviations. The section also describes the hypothesis testing process, calculations performed (e.g., pooled standard deviation, t-value, degrees of freedom), and the results obtained. The conclusion regarding the significant difference in time efficiency is discussed.

### Success/Failure Rates Analysis

The success/failure rates analysis section focuses on comparing the performance of the "Amir" and "Mine" approaches based on success and failure counts. It describes the hypothesis testing process, calculations performed (e.g., success rates, observed difference, standard error, Chi-Square value), and the results obtained. The conclusion about the difference in success rates is discussed, highlighting the lack of significant variation between the approaches.

### Conclusion

The conclusion section summarizes the main findings and conclusions drawn from the analysis. It highlights the contrasting performance of the "Amir" and "Mine" approaches in terms of time efficiency while addressing the lack of substantial variation in success rates.


