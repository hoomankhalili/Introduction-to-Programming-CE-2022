```java
public class Ex {

    public static void main(String[] args) {
        int n = Integer.parseInt(args[0]);

        for (int i = -n; i <= n; i++) {
            for (int j = -n; j <= n; j++) {
                if ((i == -j) || (i == j)) System.out.print("* ");
                else                       System.out.print(". ");
            }
            System.out.println();
        }
    }
}
```
