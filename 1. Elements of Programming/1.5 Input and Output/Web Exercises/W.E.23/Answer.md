```java
public class BallisticMotion {

    public static void main(String[] args) {
        double GRAVITATION_CONSTANT = 9.8;    // gravitational constant m/s^2
        double DRAG_COEFFICIENT = 0.002;      // drag force coefficient

        double v     = Double.parseDouble(args[0]);                    // velocity
        double theta = Math.toRadians(Double.parseDouble(args[1]));    // angle in radians

        double x = 0.0, y = 0.0;           // position
        double vx = v * Math.cos(theta);   // velocity in x direction
        double vy = v * Math.sin(theta);   // velocity in y direction

        double ax = 0.0, ay = 0.0;         // acceleration
        double t  = 0.0;                   // time
        double dt = 0.01;                  // time quantum

        // maximum distance without drag force
        double maxR = v*v / GRAVITATION_CONSTANT;
        StdDraw.setXscale(0, maxR);
        StdDraw.setYscale(0, maxR);
        StdDraw.enableDoubleBuffering();

        // loop until ball hits ground
        while (y >= 0.0) {
            v = Math.sqrt(vx*vx + vy*vy);
            ax = -DRAG_COEFFICIENT * v * vx;
            ay = -GRAVITATION_CONSTANT - DRAG_COEFFICIENT * v * vy;
            vx += ax * dt;
            vy += ay * dt;
            x  += vx * dt;
            y  += vy * dt;
            StdDraw.filledCircle(x, y, 0.25);
            StdDraw.show();
            StdDraw.pause(5);
        }
    }

}
```
