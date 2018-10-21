# CarND-Controls-PID
Self-Driving Car Engineer Nanodegree Program

## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./pid`. 

## PID Parameters
 The P, D, I parameters were chosen using maunal tuning preocess. (Starting with the values shown in the lessons)
 
 PID parameters for steering value PID Controller

 ``
 pid.Init(0.5, 0.001, 3.0);
 ``

 PID parameters for throttle value PID Controller

 ``
 pid.Init(0.9, 0.005, 5.0);
 ``
 
 ## Observation:
 
Driving around with low throttle value (0.3) was smooth, although the speed was low. When I added yet another PID controller for determining throttle value, the car oscillates while driving. Therefore I added additional check that if the steering angle is higher, then speed should be low.

## Snapshots


<img src="./images/1.png" height="400" width="800">

<img src="./images/2.png" height="400" width="800">

<img src="./images/3.png" height="400" width="800">


 
 
 

