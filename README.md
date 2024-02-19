# Welcome to My Project Files

Robotics is my passion. I first started tinkering when I was 14, with one of my earliest benchmarks being a massive [K'nex Robotic Arm](https://www.youtube.com/watch?v=M24NSTdlk6I) that sported hobby sensors and servos. From these humble beginnings, my intrigue has grown exponentially to keep pace with the fascinating realm of intelligent machines. 

## I.A.R.M. 3.0 (Interactive Autonomous Robotic Manipulator)

![IARM 3 CAD](./assets/complete_chassis.JPG)
**Behold!** My first design fabricated entirely from 3D-printed parts. The end goal is to use computer vision and A.I. to play a real-world game of chess against a human opponent...and win! To accomplish this, IARM 3.0 boasts 5 degrees of freedom (DOF) powered by stepper motors. All necessary computer vision and artificial intelligence capabilities are handled by an NVIDIA Jetson Nano and [OAK-D stereoscopic camera](https://store.opencv.ai/products/oak-d). 

![IARM 3 MOVING](./assets/IARM_DOF_test.gif)

For position control, the robot kinematics are handled by the ROS MoveIt application which interfaces with the motor drivers through an Arduino Mega 2560. Check out my Youtube [video](https://youtu.be/PcROnV9fZaA) for a quick introduction to the unique design.

## Mobile Prototyping Platform

![Mini dorito CAD](./assets/Mini_dorito_CAD.PNG)

**Behold!** Combining real-time computer vision with mobile robotic systems turns out to be a real challenge. This miniature mobile robot serves as a prototyping platform for doing just that. A Raspberry Pi/Arduino setup allows for a conservative chassis and low power consumption, while a Picamera provides live video onboard image processing. 

![Mini dorito assembled](./assets/Mini_dorito_assembled.JPG)

The primary motivation behind this design was to experiment with basic lane navigation techniques. By basic I mean entirely image-processing based; no advanced machine learning or neural networks here. Instead a plethora of basic OpenCV functions and the [RANSAC](https://hands-on.cloud/using-the-random-sample-consensus-ransac-algorithm-in-python/) algorithm were combined to allow the robot to identify lanes in a simple driving environment.
