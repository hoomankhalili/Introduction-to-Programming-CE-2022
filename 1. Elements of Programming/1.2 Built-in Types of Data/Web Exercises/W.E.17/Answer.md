```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter (x1): ");
        int x1 = sc.nextInt();
        System.out.println("Enter (y1): ");
        int y1 = sc.nextInt();

        System.out.println("Enter (x2): ");
        int x2 = sc.nextInt();
        System.out.println("Enter (y2): ");
        int y2 = sc.nextInt();

        double distance = Math.sqrt(Math.pow(y1 - y2, 2) + Math.pow(x1 - x2, 2));

        System.out.println(distance);

    }

}
```
