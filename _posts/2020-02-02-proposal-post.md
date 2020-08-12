---
title: "Project Proposal"
date: 2020-02-02  
categories: 
 - inPurdue
 - Project
--- 

## Abstract    
This project is to design an AI robot to carry out reconnaissance missions and identify whether there are enemies in the environment. The reason we're doing this is that soldiers are vulnerable on the battlefield, especially on reconnaissance missions. If the AI program can be used to replace humans to carry out reconnaissance missions, it can not only reduce the casualties of personnel but also quickly obtain the information of the enemy, which is conducive to the victory of the war. 
Our project test will be done by using a P3-AT robot. The first step of the project is to set up a network to facilitate communication between the commander and the robot and move it to the GPS coordinates set by the command. We are going to use ROS(Robot Operating System) to control and GPS module to move the robot, P3-AT. The second step is to detect objects to identify people and obstacles.We are going to use a raspberry pi with the pi camera model to be the hardware platform. We will write our program based on python to write the program and test four algorithm:   
  - Mask R-CNN  
 - Faster R-CNN  
 - Fast R-CNN  
 - YOLO V3  
Those programs were a machine learning algorithm helps us training the program to detect whether the object is human.  
After detecting the object, we will design a response system to beat back to the enemy.  

## Introduction  
Recently, the war using AI has become a big issue as the military technology competition between the U.S. and China has spread to artificial intelligence. Afterward, the military development of AI robots could determine the outcome or defeat of the war.If it is possible to detect enemies by applying AI to robots, it can also reduce the risk of actual soldiers on reconnaissance, and it has the potential to develop into more areas such as attack, hiding, and invasion.

