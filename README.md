# DAX-Training-Game-Dashboard

## Project Overview

Created 1 training game to ultilise `DAX` function for Santa where he can set an initial launch angle and velocity to see if he can hit various goal distances.


## Tech stacks used in the project
1. Power BI
2. DAX Studio
   

## Tech skills
* Creating measures and calculated columns using the `DAX` language.
* Applying 𝐜𝐨𝐧𝐝𝐢𝐭𝐢𝐨𝐧𝐚𝐥 𝐟𝐨𝐫𝐦𝐚𝐭𝐭𝐢𝐧𝐠.
* Implementing 𝐩𝐞𝐫𝐟𝐨𝐫𝐦𝐚𝐧𝐜𝐞 𝐨𝐩𝐭𝐢𝐦𝐢𝐳𝐚𝐭𝐢𝐨𝐧 techniques.
* Deploying reports to the `Power BI service`.

## Parameter Setup

All parameters are a series of numbers with their own step size.

Goal Distance – From 100 – 1000; Step size of 10
Launch Angle – From 5 to 45; Step size of 10
Velocity – From 30 to 100; Step size of 10
Mode – 0 or 1 (Representing Aim and Fire)

## Calculations

Create a table of points from 0 to 20 which will act as the incremental points as your projectile moves from point 0 to 20.  Within this table, create the following:

1. Vx (velocity in the x-direction) = Velocity*cos(Launch Angle*PI()/180)
2. Vy (velocity in the y-direction) = Velocity*sin(Launch Angle*PI()/180)
3. Max Time (time of flight) = 2 * [Vy] / 9.8
4. Max Distance = [Vx] * 2 * [Vy] / 9.8
5. Height = [Vy]*[Time]-0.5*9.8*[Time]^2
6. Distance = [Vx]*[Time]
7. Gift = unichar(127873)
8. Time = Incremental time between 0 and max time (make this dynamic in case we wanted to increase the number of points)

## DAX Training Game Dashboard

### Feel Free to use the interactive [dashboard.](https://app.powerbi.com/view?r=eyJrIjoiNTBhNGE3NjctNDU1Yy00ODI2LWE4YjUtNWJiMzE2NjJkZTEyIiwidCI6IjMxNjIzZjJjLWQ0ZTMtNDYwOS1iNTkzLWMzNjVkN2I3YmExZiJ9)

![SANTA'S SEASONAL TRAINING.png](https://github.com/PennyLi123/DAX-Training-Game-Dashboard/blob/main/SANTA'S%20SEASONAL%20TRAINING.png)


