# VerticalFarmingAutomation

A two-semester capstone project. <br>
[Paper Link](https://github.com/brucekimrokcmu/VerticalFarmingAutomation/blob/main/Vertical%20Farming%20Automation%20Spring%20Validation_report.pdf)

Our team is building a robot that traverses a vertical farming environment to pollinate and harvest tomatoes.<br>
We implemented vertical farming automation software on the Stretch-RE1 platform.<br>
We mainly used ROS as middleware and used Python to code perception, navigation, and manipulation functions on each node and implemented corresponding launch files. 
For the customized harvester and pollinator to be integrated, we modified the URDF file of the robot and the YAML file to configure motors. <br>
[Code](https://github.com/mrsd22bob) <br>

[![Full Video Link](https://user-images.githubusercontent.com/92174982/182005537-ad024d34-3d06-4e59-a782-2393c1c1064b.JPG)](https://youtu.be/rpTjnxoaoFM) <br>




I was responsible for manipulation and project management in the Spring 22 semester. <br>
>* Use head camera to detect ArUco marker
>* Subscribe to the ArUco marker topic, which is a twist coordinate published
>* Extract a constant coordinate from the subscribed ArUco marker coordinates 
>* Implement inverse kinematics using move_to_pose() Stretch ROS package by
>    * Use TF2 to conduct homogeneous transformation for the coordinate viewed at the base link of the robot
>    * measure the distance between the base link of the robot and the end of the fully retracted telescopic arm link at its lowest lift height to calculate the offset
>    * Add the offset to the desired goal positions
>* Conduct direct offset calibration to improve positional accuracy

I will be focusing on the perception part in the Fall 22 semester. <br>

**Manipulation**<br>
![Manipulation](https://user-images.githubusercontent.com/92174982/182002189-2031ef27-5600-404f-bc1f-c63e55b1242c.gif)
