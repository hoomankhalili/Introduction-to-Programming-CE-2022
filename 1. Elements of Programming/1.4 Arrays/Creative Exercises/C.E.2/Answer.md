```java
public class InversePermutation {
    public static void main(String[] args) {

        int n = args.length;

        // read in permutation
        int[] a = new int[n];
        for (int i = 0; i < n; i++)
            a[i] = Integer.parseInt(args[i]);

        // check if valid
        boolean[] exists = new boolean[n];
        for (int i = 0; i < n; i++) {
            if (a[i] < 0 || a[i] >= n || exists[a[i]])
                throw new RuntimeException("Input is not a permutation.");
            exists[a[i]] = true;
        }

        // invert
        int[] ainv = new int[n];
        for (int i = 0; i < n; i++)
            ainv[a[i]] = i;


        // print out
        for (int i = 0; i < n; i++)
            System.out.print(ainv[i] + " ");
        System.out.println();
    }
}
```
