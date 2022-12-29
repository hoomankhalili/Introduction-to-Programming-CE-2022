```java
public class Euler {

    public static void main(String[] args) {
        int n = Integer.parseInt(args[0]);

        // precompute i^5 for i = 0..n
        long[] five = new long[n+1];
        for (int i = 0; i <= n; i++)
            five[i] = (long) i * i * i * i * i;
        System.out.println("Done precomputing fifth powers");


        // now do exhaustive search
        for (int e = 1; e <= n; e++) {
            long e5 = five[e];

            // restrict search to a <= b <= c <= d <= e
            for (int a = 1; a <= n; a++) {
                long a5 = five[a];
                if (a5 + a5 + a5 + a5 > e5) break;

                for (int b = a; b <= n; b++) {
                    long b5 = five[b];
                    if (a5 + b5 + b5 + b5 > e5) break;

                    for (int c = b; c <= n; c++) {
                        long c5 = five[c];
                        if (a5 + b5 + c5 + c5 > e5) break;

                        for (int d = c; d <= n; d++) {
                            long d5 = five[d];
                            if (a5 + b5 + c5 + d5  > e5) break;
                            if (a5 + b5 + c5 + d5 == e5)
                            System.out.println(a + "^5 + " + b + "^5 + " + c + "^5 + " + d + "^5 = " + e + "^5");
                        }
                    }
                }
            }
        }
    }
}
```
