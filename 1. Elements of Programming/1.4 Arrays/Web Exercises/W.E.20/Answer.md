```java

public class ZipBarCoder {

    public static void main(String[] args) {
        int n = Integer.parseInt(args[0]);
        int[] digits = new int[6];
        int[][] code = { { 1, 1, 0, 0, 0 },
                         { 0, 0, 0, 1, 1 },
                         { 0, 0, 1, 0, 1 },
                         { 0, 0, 1, 1, 0 },
                         { 0, 1, 0, 0, 1 },
                         { 0, 1, 0, 1, 0 },
                         { 0, 1, 1, 0, 0 },
                         { 1, 0, 0, 0, 1 },
                         { 1, 0, 0, 1, 0 },
                         { 1, 0, 1, 0, 0 } };

        // extract digits
        for (int i = 1; i <= 5; i++) {
            digits[i] = n % 10;
            n /= 10;
        }

        // compute check digit
        int checkdigit = 0;
        for (int i = 1; i <= 5; i++)
            checkdigit += digits[i];
        digits[0] = checkdigit % 10;

        // print barcode
        System.out.println("*****");
        for (int i = 5; i >= 0; i--)
            for (int j = 0; j < 5; j++)
                if (code[digits[i]][j] == 1) System.out.println("*****");
                else                         System.out.println("**");
        System.out.println("*****");
    }
}
```
