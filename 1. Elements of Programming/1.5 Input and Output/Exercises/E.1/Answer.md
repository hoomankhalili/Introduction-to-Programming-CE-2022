```java
import java.util.Scanner;

public class MaxMin {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        System.out.println("Enter the number of input numbers :");
        int count = input.nextInt();

        System.out.println("Enter the number :");
        int max = input.nextInt();
        int min = max;

        for (int i = 1 ; i < count ; i++) {

            System.out.println("Enter the number :");
            int value = input.nextInt();

            if (value > max) max = value;
            if (value < min) min = value;
        }

        System.out.println("maximum  = " + max + ", minimum = " + min);
    }
}
```
