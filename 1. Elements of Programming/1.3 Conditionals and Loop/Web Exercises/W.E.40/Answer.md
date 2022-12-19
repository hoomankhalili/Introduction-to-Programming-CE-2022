```java
public class NPerLine {
    public static void main(String[] args) {
        int n = Integer.parseInt(args[0]);
        int numberOfLines = 1000 / n;
        int number = 1;
        for (int i = 0; i < numberOfLines; i++) {
            for (int j = 0; j < n; j++) {
                System.out.print(number);
                number++;
                if (number / 10 >= 10)
                    System.out.print(" ");
                else if (number / 10 >= 1)
                    System.out.print("  ");
                else if (number / 10 >= 0)
                    System.out.print("   ");
            }
            System.out.println();
        }
    }
}
```
