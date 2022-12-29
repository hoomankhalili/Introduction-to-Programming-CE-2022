```java
import java.util.Scanner;

public class State {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        int n = Integer.parseInt(args[0]);
        double[] a = new double[n];

        for (int i = 0; i < n; i++) {
            System.out.println("Enter a number :");
            a[i] = input.nextDouble();
        }

        double sum = 0.0;
        for (int i = 0; i < n; i++) {
            sum += a[i];
        }
        double mean = sum / n;

        double sum2 = 0.0;
        for (int i = 0; i < n; i++) {
            sum2 += (a[i] - mean) * (a[i] - mean);
        }
        double stddev = Math.sqrt(sum2 / (n - 1));

        System.out.println("Mean                      = " + mean);
        System.out.println("Sample standard deviation = " + stddev);
    }
}
```
