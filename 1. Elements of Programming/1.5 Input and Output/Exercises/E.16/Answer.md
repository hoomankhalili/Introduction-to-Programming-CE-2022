```java
import java.util.Scanner;

public class Centroid {
    public static void main(String[] args) throws Exception {
        
        Scanner input = new Scanner(System.in);

        double x = 0;
        double y = 0;
        double m = 0;

        System.out.println("Enter the number of objects : ");
        int count = input.nextInt();

        for (int i = 0 ; i < count ; i++) {

            System.out.println("Enter the value of x" + i + " :");
            int xi = input.nextInt();
            System.out.println("Enter the value of y" + i + " :");
            int yi = input.nextInt();
            System.out.println("Enter the value of m" + i + " :");
            int mi = input.nextInt();

            m += mi;
            x += mi * xi;
            y += mi * yi;
        }

        x /= m;
        y /= m;

        System.out.println("The value of the center of mass is equal to : " + "(" + x + ", " + y + ", " + m + ")");
    }
}
```
