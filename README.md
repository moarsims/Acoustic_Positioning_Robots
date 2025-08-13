# Acoustic_Positioning_Robots
A Precise Positioning and Guidance System for Robots Using Acoustic Trilateration

This was my capstone final year undergraduate project. It was designed to precisely locate a robot inside an indoor environment tiled by a local coordinate system and control it to navigate that space. Basically indoor GPS with sound.

The system consists of speakers mounted on robots and microphones mounted in stationary locations in the indoor environment (base stations).

At time of reading, the system can only measure the linear distance from one robot to one microphone to an accuracy of five centimeters (1D localisation).

How it works is as follows:
- The user specifies the robot they want to move
- The base stations send a chirp command signal over a 433MHz link to the specific robot and starts a microsecond timer
- The robot's speaker releases a chirp at 5000 Hz for 100 ms
- The base station stops the clock when the sound arrives and records the time elapsed while the sound was in flight
- The base station uses this elapsed time and the speed of sound to calculate the robot's distance

Future development aims to increase the number of microphones inorder to actually locate the robot in 2D space.



NB: Incomplete
