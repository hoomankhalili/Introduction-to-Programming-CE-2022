```java
public class MostLikelyRoll {

    public static void main(String[] args) {
        int SIDES = 6;
        int TARGET = 12;
        int trials = Integer.parseInt(args[0]);     // number of trials

        int[] freq = new int[TARGET + SIDES + 1];

        for (int t = 1; t <= trials; t++) {
            int sum = 0;
            while (sum <= TARGET) {
                int die = 1 + (int) (Math.random() * SIDES);
                sum += die;
            }
            freq[sum]++;
        }

        for (int i = TARGET + 1; i <= TARGET + SIDES; i++) {
            double fraction = 1.0 * freq[i] / trials;
            System.out.println(i + ": " + fraction);
        }
    }
}

```
