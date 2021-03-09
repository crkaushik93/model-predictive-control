# MPC- Model Predictive Control


## Project Description

### Overview

**Model predictive control (MPC)** is a process control that depends on the dynamic or kinematic model of the vehicle.
It has the ability to predict the future events and can control the actions. Also, future time steps are considered depending the time slots provided.

The MPC controller framework consists in four main components:
 - **Trajectory** which is considerd during optimization. It is calculated by a number of time steps ***N*** spaced out by a time ***dt***.
 
 - **Vehicle Model**, which is the set of equations that describes system behavior. Some of the constraints considered are 
   - **x** car position along x axis
   - **y** car position along y axiz
   - **psi** be the car's moving direction
   - **v** velosity of car
   - **cte** cross-track error
   - **epsi** orientation error
   
 - **Contraints** necessary to model contrants in actuators' respose. 
   - **steering**: bounded in range [-25°, 25°]
   - **acceleration**: bounded in range [-1, 1] from full brake to full throttle
   
 - **Cost Function** on whose optimization is based the whole control process. Usually cost function is made of the sum of different terms.
 - 
