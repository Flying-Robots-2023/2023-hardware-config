# Configuring RaspberryPi 4b  

To enabled the connection between RaspberryPi 4b and the Depth Camera Realsense 435d, we had to follow directelly some instructions from [Ai_Demos_RPi](https://github.com/datasith/Ai_Demos_RPi/wiki/Raspberry-Pi-4-and-Intel-RealSense-D435). 

Then we followd the instructions of the [realsense-ros-github-page](https://github.com/IntelRealSense/realsense-ros/tree/ros1-legacy) for ros1-legacy. 

Before the step ``` catkin build``` in our catkin workspace to compile the realsense-ros repository, we had to add another package inside ``` ~/catkin_ws/src/ ```. It was the [ddynamic-reconfigure](https://github.com/pal-robotics/ddynamic_reconfigure/tree/kinetic-devel) package that was a deppendendy of realsense-ros.
Onde that was done we had the workspace builded and then, after that we added the  realsense-ros package, so then we could compile it as done on the instructions. 

To test the work done, we again followed the tutorial of the Realsense Repository. 
