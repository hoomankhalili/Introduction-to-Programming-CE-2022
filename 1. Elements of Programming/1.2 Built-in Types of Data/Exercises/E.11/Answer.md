```java
import java.util.Scanner;

public class Main {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.println("Enter (d): ");
        int d = sc.nextInt();
        System.out.println("Enter (m): ");
        int m = sc.nextInt();

        if (3 < m && m < 6){
            System.out.println(true);

        } else if (m == 3 && 20 <= d) {
            System.out.println(true);

        } else if (m == 6 && d <= 20) {
            System.out.println(true);

        } else {
          System.out.println(false);

        }

    }

}
```
