# HURBA: ROS and Gazebo tutorial I.

[//]: # (Image References)

[image1]: ./documentation/gazebo.png "Gazebo"
[image2]: ./documentation/frames.png "TF"
[image3]: ./documentation/rosgraph.png "Graph"
[image4]: ./documentation/rviz.png "RViz"

### Dependencies:
- ROS Melodic
- Gazebo 9
- RViz
- Teleop twist keyboard

### Project build instrctions:
1. Clone this repo inside the `src` folder of a catkin workspace:
`git clone https://github.com/hungarianrobot/Project-1-Gazebo-Basics`
3. Build workspace: `catkin_make`
4. Source environment: `source devel/setup.bash` 
5. Start the Gazebo simulation and RViz: `roslaunch my_robot world.launch`
6. Start the Teleop package: `rosrun teleop_twist_keyboard teleop_twist_keyboard.py`

![alt text][image1]
![alt text][image4]
![alt text][image3]
![alt text][image2]

### Project structure:
```bash
tree
Project-1-Gazebo-Basics
├── README.md
├── documentation
│   ├── frames.png
│   ├── gazebo.png
│   ├── rosgraph.png
│   └── rviz.png
└── hurba_robot
    ├── CMakeLists.txt
    ├── launch
    │   ├── robot_description.launch
    │   ├── teleop.launch
    │   └── world.launch
    ├── meshes
    │   ├── chassis.SLDPRT
    │   ├── chassis.STEP
    │   ├── chassis.dae
    │   ├── hokuyo.dae
    │   ├── wheel.SLDPRT
    │   ├── wheel.STEP
    │   └── wheel.dae
    ├── package.xml
    ├── rviz
    │   └── basic_view.rviz
    ├── urdf
    │   ├── hurba_robot.gazebo
    │   └── hurba_robot.xacro
    └── worlds
        ├── basic_world.world
        └── empty.world
```

