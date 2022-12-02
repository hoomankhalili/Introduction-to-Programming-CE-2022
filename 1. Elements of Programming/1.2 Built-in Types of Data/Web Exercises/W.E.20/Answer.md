```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter (a): ");
        int a = sc.nextInt();
        System.out.println("Enter (b): ");
        int b = sc.nextInt();
        System.out.println("Enter (c): ");
        int c = sc.nextInt();

        double s = (double) (a + b + c) / 2;

        double area = Math.sqrt(s * (s-a) * (s-b) * (s-c));

        System.out.println(area);

    }

}
```
