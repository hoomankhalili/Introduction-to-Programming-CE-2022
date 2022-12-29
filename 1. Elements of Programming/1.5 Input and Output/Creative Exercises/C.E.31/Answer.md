```java
public class Spirograph {
    public static void main(String[] args) {

        double R = Double.parseDouble(args[0]);;
        double r = Double.parseDouble(args[1]);;
        double a = Double.parseDouble(args[2]);; 
        
        double min = -(2 * R + 2 * r);
        double max = 2 * R + 2 * r;

        StdDraw.setXscale(min, max);
        StdDraw.setYscale(min,max);
        StdDraw.enableDoubleBuffering(); 

        for (double t = 0.0; t < 80; t += 0.02)  {

            double x = (R + r) * Math.cos(t) - (r + a) * Math.cos(((R + r)/r) * t);
            double y = (R + r) * Math.sin(t) - (r + a) * Math.sin(((R + r)/r) * t);

            StdDraw.setPenColor(StdDraw.BLACK);
            StdDraw.filledCircle(x, y, 4);
            StdDraw.show();
            StdDraw.pause(20);
        }
    }
}
```
