# RT2 Assignment
# docs
# Second
## Robot Goal Planning and Visualization
This directory contains code to satisfy some features such as
-  Some buttons for handling the motion of the robot
-  A plot with the robot’s position and targets’ positions
-  A text box with the distance of the closest obstacle
-  A plot for the number of reached/not-reached targets

The system allows users Jupyter Notebook to input goal positions, send goals to the robot, visualize the robot's goals on a scatter plot, monitor the closest obstacle distance detected by the robot and plot the numer of reached or canceled obstacles.

## Prerequisites

- ROS 
- Python 3
- IPython Widgets
- matplotlib
- actionlib
- assignment_2_2022 package
- sensor_msgs package
- nav_msgs package
- std_srvs package

## Usage

1. Clone the repository and navigate to the project directory.
     https://github.com/CarmineD8/assignment_2_2022 
3. Launch the ROS environment.
4. Launch the Jupyter Notebook.
     ``` jupyter notebook```
6. Run the following command to execute the goal planning and visualization system:
     ```roslaunch assignment_2_2022 assignment1.launch ```
6. Use the input fields to enter the X and Y positions for the robot's goal.
7. Click the "Send Goal" button to send the goal to the robot.
8. Click the "Cancel Goal" button to cancel the active goal.
9. The scatter plot will display the robot's goal positions in real-time.
10. The "Closest Obstacle Distance" value will be updated based on the laser scan data received by the robot.
11. The numer of reached or canceled target will be ploted on the screen.



# Third
## Statistical Analysis Report

This directory contains a statistical analysis report comparing the time efficiency and success/failure rates between two approaches: "Amir" and "Mine". The report presents the experimental design, hypothesis testing, calculations, and results for both factors.

## Abstract

The abstract provides a summary of the report, highlighting the purpose of the analysis and the main findings. It mentions the significance level used for hypothesis testing.

## Introduction

The introduction section introduces the context and objectives of the report. It explains the goal of evaluating and comparing the time efficiency and success/failure rates between the "Amir" and "Mine" approaches.

## Experimental Design

The experimental design section outlines the parameters of the experiment, including the map configurations, numbers of tokens, and the number of tests conducted. It provides essential information about the data collection process.

## Time Efficiency Analysis

This section presents the analysis of time efficiency for both the "Amir" and "Mine" approaches. It includes the statistical parameters, such as sample sizes, means, and standard deviations. The section also describes the hypothesis testing process, calculations performed (e.g., pooled standard deviation, t-value, degrees of freedom), and the results obtained. The conclusion regarding the significant difference in time efficiency is discussed.

## Success/Failure Rates Analysis

The success/failure rates analysis section focuses on comparing the performance of the "Amir" and "Mine" approaches based on success and failure counts. It describes the hypothesis testing process, calculations performed (e.g., success rates, observed difference, standard error, Chi-Square value), and the results obtained. The conclusion about the difference in success rates is discussed, highlighting the lack of significant variation between the approaches.

## Conclusion

The conclusion section summarizes the main findings and conclusions drawn from the analysis. It highlights the contrasting performance of the "Amir" and "Mine" approaches in terms of time efficiency while addressing the lack of substantial variation in success rates.

Please refer to the report for detailed information and results.


