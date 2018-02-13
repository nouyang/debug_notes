Compile 17.10 ROS
http://answers.ros.org/question/277021/ros-lunar-on-ubuntu-1710/it@github.com:nouyang/debug_notes.git


Step by step bash
https://gist.github.com/gavanderhoorn/28062c9ba78eed6cb098569a5b886896

I guess I should install docker...
https://docs.docker.com/install/linux/docker-ee/ubuntu/#install-docker-ee


=====

# Arduino and Processing
Okay meanwhile let's get arduino 1.8.5 (latest version, not apt get version)


Hmm. Bildr library is sad. Well it is from 6 years ago
(processing fails with some king of opengl error)
http://bildr.org/2012/03/stable-orientation-digital-imu-6dof-arduino/
The arduino part of it compiles fine.
Maybe just debug the processing side then. Shouldn't be too difficult.

Let's try Sparkfun directly
https://www.sparkfun.com/products/10121
https://github.com/sparkfun/IMU_Digital_Combo_Board.git


====

Well. Compiling ROS doesn't seem to have worked (some catkin_make doesn't even
run).

Let's try docker instead.
nrw@chai:~/Documents/projects_Spring2018$ sudo docker build -t roslunar .

