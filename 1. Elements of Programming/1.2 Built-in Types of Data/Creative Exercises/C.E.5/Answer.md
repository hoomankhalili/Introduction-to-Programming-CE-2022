```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter the first number: ");
        int a = sc.nextInt();

        System.out.println("Enter the second number: ");
        int b = sc.nextInt();

        System.out.println("Enter the third number: ");
        int c = sc.nextInt();

        int x = Math.min(a, b);
        int min = Math.min(x, c);

        int y = Math.max(a, b);
        int max = Math.max(y, c);

        int mid = a + b + c - min - max;

        System.out.println(min);
        System.out.println(mid);
        System.out.println(max);

    }

}
```
