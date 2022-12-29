***Projectile motion with drag.*** Write a program BallisticMotion.java that plots the trajectory of a ball that is shot with velocity v at an angle theta. Account for gravitational and drag forces. Assume that the drag force is proportional to the square of the velocity. Using Newton's equations of motions and the Euler-Cromer method, update the position, velocity, and acceleration according to the following equations:
```java
v  = sqrt(vx*vx + vy*vy) 
ax = - C * v * vx          ay = -G - C * v * vy
vx = vx + ax * dt          vy = vy + ay * dt
 x =  x + vx * dt           y =  y + vy * dt
```
Use G = 9.8, C = 0.002, and set the initial velocity to 180 and the angle to 60 degrees.
