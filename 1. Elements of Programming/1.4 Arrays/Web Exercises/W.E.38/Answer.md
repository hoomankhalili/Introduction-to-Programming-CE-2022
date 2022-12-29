```java
import java.util.Random;

public class Rolling5Dices {
    public static void main(String[] args) {
        Random r = new Random();
        int low = 1;
        int high = 6;
        int result1 = r.nextInt(high-low) + low;
        int result2 = r.nextInt(high-low) + low;
        int result3 = r.nextInt(high-low) + low;
        int result4 = r.nextInt(high-low) + low;
        int result5 = r.nextInt(high-low) + low;
        if (result1==result2 && result2==result3 &&
            result3==result4 && result4==result5) {
                System.out.println("Yahtzee");
            } else {
                System.out.println("Try again.");
            }
    }
}

```
