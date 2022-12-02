```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter (x): ");
        int x1 = sc.nextInt();
        System.out.println("Enter (y): ");
        int y1 = sc.nextInt();

        int x0 = 0;
        int y0 = 0;

        double distance = Math.sqrt(Math.pow(y1 - y0, 2) + Math.pow(x1 - x0, 2));

        System.out.println(distance);

    }

}
```
