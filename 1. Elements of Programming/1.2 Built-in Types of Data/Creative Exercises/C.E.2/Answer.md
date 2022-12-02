```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter (x): ");
        int x = sc.nextInt();

        System.out.println("Enter (y): ");
        int y = sc.nextInt();

        double r = Math.sqrt(Math.pow(x, 2) + Math.pow(y, 2));

        double teta = Math.atan2(y, x);

        System.out.println("(r = " + r + " , " + "teta = " + teta + ")");

    }

}
```
