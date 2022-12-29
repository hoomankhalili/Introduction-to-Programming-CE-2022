```java
public class WindChill {
    public static void main(String[] args) {
        double t = Double.parseDouble(args[0]);
        double v = Double.parseDouble(args[1]);
        if (v < 3 || v > 110 || t > 50 || t < -50)
            System.out.println("Error: Input out of range");
        else {
            double w = 35.74 + 0.6215 * t + (0.4275 * t - 35.75) * Math.pow(v, 0.16);
            System.out.println("Temperature = " + t);
            System.out.println("Wind speed  = " + v);
            System.out.println("Wind chill  = " + w);
        }
    }

}
```
