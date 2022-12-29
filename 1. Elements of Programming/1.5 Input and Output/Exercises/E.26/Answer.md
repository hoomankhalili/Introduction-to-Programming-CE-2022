```java
public class Circles {
    public static void main(String[] args) {

        int circlesNum = Integer.parseInt(args[0]);
        double probability  = Double.parseDouble(args[1]);
        double minRadius = Double.parseDouble(args[2]);
        double maxRadius = Double.parseDouble(args[3]);

        StdDraw.setXscale(0, 1.0);
        StdDraw.setYscale(0, 1.0);

        for (int i = 0; i < circlesNum; i++) {

            boolean val = Math.random() < probability;

            double range = maxRadius - minRadius;
            double radius = (Math.random() * range) + minRadius;

            if ((minRadius <= radius) && (radius <= maxRadius)) {

                if (val) StdDraw.setPenColor(StdDraw.BLACK);
                else     StdDraw.setPenColor(StdDraw.WHITE);

                double x = Math.random();
                double y = Math.random();

                StdDraw.filledCircle(x, y, radius);
            }
        }
    }
}
```
