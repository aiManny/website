# Welcome to My Project Files

Robotics is my passion. I started building my own contraptions at the age of 14, using mostly plastic construction pieces. One of my earliest robots was a massive [K'nex Robotic Arm](https://www.youtube.com/watch?v=M24NSTdlk6I) that sported basic ultrasonic sensors and hobby motors. Since then, the robotics field has grown in applications and my intrigue has expanded with it. 

## I.A.R.M. 3.0 (Interactive Autonomous Robotic Manipulator)

![IARM 3 CAD](./assets/complete_chassis.JPG)
Generation 3 of my Interactive Autonomous Robotic Manipulators (I.A.R.M.), this initiative is my first design fabricated entirely from 3D-printed parts. The end state is equally as ambitious; to employ machine learning techniques in order to play chess against a human opponent in real-time...and win! To accomplish this, the IARM 3.0 chassis contrains 5 degrees of freedom (DOF) powered by stepper motors. All necessary computer vision and artificial intelligence capabilities are handled by an NVIDIA Jetson Nano and [OAK-D stereoscopic camera](https://store.opencv.ai/products/oak-d). 

![IARM 3 ASSEMBLED](./assets/IARM3_assembled_lidless.PNG)

For position control, the robot kinematics are handled by the ROS MoveIt application which interfaces with the motor drivers through an Arduino Mega 2560. An introduction to the full design can be found ![here](link_to_YouTube_channel_video).

## Mobile Prototyping Platform

![Mini dorito CAD](./assets/Mini_dorito_CAD.PNG)

Combining real-time computer vision with mobile robotic systems turns out to be a real challenge. This miniature mobile robot serves as a prototyping platform for doing just that. A Raspberry Pi/Arduino setup allows for a conservative chassis and low power consumption, while a Picamera provides live video onboard image processing. 

![Mini dorito assembled](./assets/Mini_dorito_assembled.JPG)

The primary motivation behind this design was to experiment with basic lane navigation techniques. By basic I mean entirely image-processing based; no advanced machine learning or neural networks here. Instead a plethora of basic OpenCV functions and the [RANSAC](https://hands-on.cloud/using-the-random-sample-consensus-ransac-algorithm-in-python/) algorithm were combined to allow the robot to identify lanes in a simple driving environment.
