```java
public class Oscilloscope {

    public static void main(String[] args) {

        StdDraw.setXscale(-1, +1);
        StdDraw.setYscale(-1, +1);
        StdDraw.enableDoubleBuffering();

        double aX    = Double.parseDouble(args[0]);    // amplitudes
        double aY    = Double.parseDouble(args[1]);
        double wX   = Double.parseDouble(args[2]);    // angular frequencies
        double wY   = Double.parseDouble(args[3]);
        double tX = Double.parseDouble(args[4]);    // phase factors
        double tY = Double.parseDouble(args[5]);

        // convert from degrees to radians
        tX = Math.toRadians(tX);
        tY = Math.toRadians(tY);

        for (double t = 0.0; t < 10; t += 0.0001) {

            double x = aX * Math.sin(wX * t + tX);
            double y = aY * Math.sin(wY * t + tY);

            StdDraw.point(x, y);
            StdDraw.show();
            StdDraw.pause(10);
        }
    }

}
```
