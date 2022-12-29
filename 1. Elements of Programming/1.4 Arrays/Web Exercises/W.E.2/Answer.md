```java
import java.util.Scanner;

public class aboveaverage {
    public static void main(String[] args) {
        int n = Integer.parseInt(args[0]);
        Scanner s = new Scanner(System.in);
        int arr[] = new int[n];
        double mean = 0;
        for (int i = 0; i < n; i++) {
            int t = s.nextInt();
            mean += t;
            arr[i] = t;
        }
        mean /= n;
        for (int i = 0; i < n; i++) {
            if (arr[i] > mean) {
                System.out.println(arr[i] - mean);
            }
        }
    }
}

```
