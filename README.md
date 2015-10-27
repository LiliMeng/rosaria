
For information on how to use RosAria, see <http://wiki.ros.org/ROSARIA>,
especially <http://wiki.ros.org/ROSARIA/Tutorials/How to use ROSARIA>.

Documentation on PowerBot and RosAria Connection: https://docs.google.com/document/d/1v6PMLPHarDuJ0K1XRWxKLU_ukU1tzfbbpdLlDDvNq08/edit?usp=sharing


1.Turn on the power and plug in the USB
2. check out which USB port we are using right now
$cd/dev 
$list
you could find out the ttyUSB0 or ttyUSB1
change the user access to the USB port. $sudo chmod a+rw /dev/ttyUSB0 if you are using ttyUSB0 or using  $sudo chmod a+rw /dev/ttyUSB1 is you are using ttyUSB1
3. $roscore 
4. $rosrun rosaria RosAria _port:=/dev/ttyUSB0  if the powerbot is connected to the USB0 of the laptop. Currently the robot is ready to run
5.$rostopic list to see all the rostopics
6$rostopic echo /RosAria/pose if we would like to check the pose information
7$rviz  add odometry topic to view the odometry information in the rviz
