```java
public class Blackjack {

    public static void main(String[] args) {
        boolean Y = true;
        boolean N = false;
        boolean I = false;     // irrelevant, never used

        int x = Integer.parseInt(args[0]);
        int y = Integer.parseInt(args[1]);
        int z = Integer.parseInt(args[2]);

        // split[i][j] = should you split with (i, i) if dealer is showing j
        boolean[][] split = {
            { I, I, I, I, I, I, I, I, I, I, I },
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  A,  A
            { I, N, Y, Y, Y, Y, Y, Y, N, N, N },      //  2,  2
            { I, N, Y, Y, Y, Y, Y, Y, N, N, N },      //  3,  3
            { I, N, N, N, N, Y, Y, N, N, N, N },      //  4,  4
            { I, N, N, N, N, N, N, N, N, N, N },      //  5,  5
            { I, N, Y, Y, Y, Y, Y, N, N, N, N },      //  6,  6
            { I, N, Y, Y, Y, Y, Y, Y, N, N, N },      //  7,  7
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  8,  8
            { I, N, Y, Y, Y, Y, Y, N, Y, Y, N },      //  9,  9
            { I, N, N, N, N, N, N, N, N, N, N },      // 10, 10
        };

        // soft[i][j] = should you hit with (A, i) if dealer is showing j
        boolean[][] soft  = {
            { I, I, I, I, I, I, I, I, I, I, I },
            { I, I, I, I, I, I, I, I, I, I, I },      //  A,  A
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  A,  2
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  A,  3
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  A,  4
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  A,  5
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  A,  6
            { I, Y, N, N, N, N, N, N, N, Y, Y },      //  A,  7
            { I, N, N, N, N, N, N, N, N, N, N },      //  A,  8
            { I, N, N, N, N, N, N, N, N, N, N },      //  A,  9
            { I, N, N, N, N, N, N, N, N, N, N },      //  A, 10
        };

        // soft[i][j] = should you hit with total = i if dealer is showing j
        boolean[][] hard  = {
            { I, I, I, I, I, I, I, I, I, I, I },      //  0
            { I, I, I, I, I, I, I, I, I, I, I },      //  1
            { I, I, I, I, I, I, I, I, I, I, I },      //  2
            { I, I, I, I, I, I, I, I, I, I, I },      //  3
            { I, I, I, I, I, I, I, I, I, I, I },      //  4
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  5
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  6
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  7
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  8
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      //  9
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      // 10
            { I, Y, Y, Y, Y, Y, Y, Y, Y, Y, Y },      // 11
            { I, Y, Y, Y, N, N, N, Y, Y, Y, Y },      // 12
            { I, Y, N, N, N, N, N, Y, Y, Y, Y },      // 13
            { I, Y, N, N, N, N, N, Y, Y, Y, Y },      // 14
            { I, Y, N, N, N, N, N, Y, Y, Y, Y },      // 15
            { I, Y, N, N, N, N, N, Y, Y, Y, Y },      // 16
            { I, N, N, N, N, N, N, N, N, N, N },      // 17
            { I, N, N, N, N, N, N, N, N, N, N },      // 18
            { I, N, N, N, N, N, N, N, N, N, N },      // 19
        };

        // if y is an ace, flip cards
        if (y == 1) {
            y = x;
            x = 1;
        }

        // split
        if (x == y && split[x][z])
            System.out.println("Split");

        // a single ace
        else if (x == 1) {
            if (soft[y][z]) System.out.println("Hit");
            else            System.out.println("Stick");
        }

        // no ace and did not split
        else {
            if (hard[x+y][z]) System.out.println("Hit");
            else              System.out.println("Stick");
        }

    }
}
```
