**Color Detection Bot**

This is a ROS2 package for a robot that searches an environment, looks for colored items, and reports their location using ROS2 middleware. The robot uses its sensors (camera and LiDAR) and actuators (wheels) to guide itself to each item. The success of locating an item is defined as being less than 1 meter from the item and indicating that it has found an object.



**How to Start the System**

Clone the repository:
`git clone https://github.com/yourusername/color-detection-bot.git`

Build the package:
`cd color-detection-bot 
colcon build`

Source the setup script:
`. install/setup.bash`

Launch the robot:
`ros2 launch color_detection_bot color_detection_bot.launch.py`

Once the robot is launched, it will begin searching for colored objects in its environment. When it detects an object, it will stop and turn away from the object, indicating that it has found an object. The location of the object can be obtained by subscribing to the ‘object_location’ topic.
