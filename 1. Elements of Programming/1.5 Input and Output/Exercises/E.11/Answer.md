```java
import java.util.Scanner;

public class WordCount {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);

        System.out.println("Enter your text :");
        String text = input.nextLine();

        int count = 0;
        for (int i = 0 ; i < text.length() ; i++) {

            if (text.charAt(i) == ' ') count++;
        }
        if (text.length() > 0) count++;

        System.out.println("number of words  = " + count);
    }
}
```
