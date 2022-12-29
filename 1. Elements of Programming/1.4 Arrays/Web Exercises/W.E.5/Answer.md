```java
import java.util.Random;
import java.util.Scanner;
import java.util.concurrent.ThreadLocalRandom;
import java.util.stream.IntStream;

public class MyBeer {
    Scanner s = new Scanner(System.in);
    Random r = new Random();
    int n = s.nextInt();
    for (int i = 0; i < 1000; i++) {
        int[] ar = IntStream.range(0, n).toArray();
        Random rnd = ThreadLocalRandom.current();
        for (int i = ar.length - 1; i > 0; i--) {
            int index = rnd.nextInt(i + 1);
            // Simple swap
            int a = ar[index];
            ar[index] = ar[i];
            ar[i] = a;
        }
        int count = 0;
        for (int i = 0; i < n; i++) {
            if (ar[i] == i) count++;
        }
        System.out.println(count);

    }
    
}
```
