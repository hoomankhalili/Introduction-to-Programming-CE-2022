```java
import java.util.Arrays;
import java.util.Scanner;

public class Scheduling {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int n = s.nextInt();
        int a[] = new int[n];
        for (int i = 0; i < n; i++) {
            int t = s.nextInt();
            a[i] = t;
        }
        Arrays.sort(a);
        int cost = 0;
        for (int i = 0; i < n; i++) {
            if (a[i] < i) {
                cost++;
            }
        }
        System.out.println(cost * 1000);
    }
}

```
