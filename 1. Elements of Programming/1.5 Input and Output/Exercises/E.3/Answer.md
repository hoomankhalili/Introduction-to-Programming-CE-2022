```java
import java.util.Scanner;

public class LongestRun {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.println("Enter the sequence length :");
        int length = input.nextInt();

        System.out.println("Enter the sequence :");
        int prev = input.nextInt();
        int count = 1;
        int best      = prev;
        int bestCount = count;

        for (int i = 0 ; i < length ; i++){

            int current = input.nextInt();

            if (current == prev) count++;
            
            else {

                prev = current;
                count = 1;
            }

            if (count > bestCount) {

                bestCount = count;
                best      = current;
            }
        }

        System.out.println("Longest run: " + bestCount + " consecutive " + best + "s");
    }
}
```
