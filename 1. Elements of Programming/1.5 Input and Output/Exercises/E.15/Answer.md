```java
import java.util.Scanner;

public class Closest {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        double x = Double.parseDouble(args[0]);
        double y = Double.parseDouble(args[1]);
        double z = Double.parseDouble(args[2]);

        double bestX = Double.NaN;
        double bestY = Double.NaN;
        double bestZ = Double.NaN;
        double bestDis = Double.POSITIVE_INFINITY;

        System.out.println("Enter the number of input points :");
        int count = input.nextInt();

        for (int i = 0 ; i < count ; i++){

            System.out.println("Enter the value of x" +i+ " :");
            double xi = input.nextDouble();
            System.out.println("Enter the value of y" +i+ " :");
            double yi = input.nextDouble();
            System.out.println("Enter the value of z" +i+ " :");
            double zi = input.nextDouble();

            double dis = (x - xi) * (x - xi) + (y - yi) * (y - yi) + (z - zi) * (z - zi);

            if (dis < bestDis) {

                bestX = xi;
                bestY = yi;
                bestZ = zi;
                bestDis = dis;
            }
        }

        System.out.printf("Closest point = (%f, %f, %f)\n", bestX, bestY, bestZ);
    }
}
```
