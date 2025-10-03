---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
redirect_from:
  - /research
---

# Education Experience
**Master of Philosophy - the Hong Kong University of Science and Technology**
  ***advisor : prof. Fumin Zhang***

  ***Fully autonomous docking system suitable for small sized vessels***

  I’m currently building an autonomous docking system for small vessels. The system is organized into four layers—perception, user interaction, path planning, and motion control—and my work focuses on improving the path planning and motion control components.

  - **Objective & scenarios:** Achieve end-to-end autonomous docking in narrow waters such as marinas and around buoys, covering far-field guidance, obstacle-aware approach, terminal alignment, and final berthing, with an emphasis on practical deployment and reliability.

  - **Path planning layer:** We combine A* with Reeds–Shepp to search for low-risk routes, integrating costs for obstacle clearance, channel deviation, and steering effort. This balances exploration with efficiency to rapidly generate a reference path. ![rs astar path](https://ennishsu.github.io/images/rsastar.jpg)
  - **Motion control layer:** The motion control component is built on a simplified 3-DoF vessel dynamics model, with constraints on thrust, rudder angle, angular rate, and minimum safety distance. We use NMPC to track the reference path and convert it into control commands, improving convergence and disturbance rejection. In addition, because environmental effects on the water—such as wind and current—are difficult to model, we will train a model to compensate disturbances online within the NMPC prediction model to improve path-tracking accuracy.
  
  The project is currently in the simulation–validation stage, using the VRX simulator (built on ROS 2 and Gazebo) for experiments. A selection of results is shown below.

  <iframe src="https://ennishsu.github.io/images/vrx.MOV" width="480" height="320" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> 
  </iframe>

**Bachelor - South China University of Technology**
- Undergraduate Thesis : Fine-grained Classification of Bone Marrow Cells Using Deep Learning **advisor : prof. Weining Wang**
    - Utilized the Pytorch framework
    - Evaluate and contrast three cell classification algorithmic models: the [Resnet50](https://github.com/EnnisHsu/Cell_Resnet.git), Pairwise Interaction Network, and the Attention Pyramid Model
    - Conducted an analysis of diverse data augmentation strategies, encompassing conventional methods, [Progressive GAN](https://github.com/EnnisHsu/progressive-gan-pytorch.git),and [Style GAN2](https://github.com/EnnisHsu/stylegan2-ada-pytorch.git), to ascertain their impact on model performance.
    ![StyleGAN2_pic](https://ennishsu.github.io/images/StyleGAN2_cell.jpg)
    - Pyramid Model with the advanced features of Style GAN2, culminating in an improvement in the fine-grained classification accuracy of bone marrow cells

- SCUT Robotics Lab - RoboMaster National University Student Robot Competition **advisor : prof. Dong Zhang**
    - chief developer of Engineer Robot and [Robot with Manipulator](https://github.com/EnnisHsu/21_TigerArm/commits/dev/)
    - Implemented motion control for the robots chassis and upper structures using CAN and serial communication protocols combined with cascaded control systems.
    - Utilized [Coppeliasim simulations](https://github.com/EnnisHsu/20_VREP_Engineer.git) and finite state machine algorithms for automating the ammunition reloading process.
    -  Achieved simulation of the six degrees of freedom in the robotic arm's joint movements using a combination of Coppeliasim simulations and Matlab computation
    - Enhanced the arm's motion smoothness using cascaded control systems and polynomial interpolation algorithms.

<iframe src="https://ennishsu.github.io/images/Enginner_Simulation.mp4" width="480" height="320" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> 
</iframe>

<iframe src="https://ennishsu.github.io/images/Tigery.mp4" width="480" height="320" scrolling="no" border="0" frameborder="no" framespacing="0" allowfullscreen="true"> 
</iframe>

- Computer Vision-Based Study Room Seat Availability System 
    - Chief developer in vision detection
    - Applied the YOLOv4 model for object detection, training the model to accurately identify occupied and available seats.
    - Integrated detection results into a database, which were then displayed on a mobile application, providing users with real-time information about seat availability.
    ![seats](https://ennishsu.github.io/images/seat.png)

<!-- <video width="640" height="480" controls>
  <source id="Engineer" src="https://ennishsu.github.io/images/Enginner_Simulation.mp4" type="video/mp4">
</videos>   -->

<!-- <video width="640" height="480" controls>
  <source id="Tigery" src="https://ennishsu.github.io/images/Tigery.mp4" type="video/mp4">
</videos> -->

