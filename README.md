# 877wCodeRepo
code repository for Vex Robotics team 877-W

Please Upload files in .zip format of the robot code, with the title indicating the purpose of this iteration 


**Coding Goals**
- Creating a program that automatically changes flywheel power depending on distance of the goal as well as rotating to the bot from any angle

Example code
```// Determine the distance to the goal
float distanceToGoal = getDistanceToGoal();

// Determine the direction of the goal relative to the robot
float directionToGoal = getDirectionToGoal();

// Calculate the power for the left and right motors based on the distance and direction to the goal
float leftPower = 0.5 * distanceToGoal + 0.5 * directionToGoal;
float rightPower = 0.5 * distanceToGoal - 0.5 * directionToGoal;

// Set the power of the left and right motors to rotate the robot in the direction of the goal
motor(PORT1).spin(forward, leftPower, percent);
motor(PORT2).spin(forward, rightPower, percent);
```
