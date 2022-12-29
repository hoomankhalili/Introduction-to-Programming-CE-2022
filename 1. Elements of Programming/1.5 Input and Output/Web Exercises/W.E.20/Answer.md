```java

import java.util.Scanner;

public class RotatingTable {
    public static void main(String[] args) {
        Scanner s = new Scanner(System.in);
        int ar[] = new int[4];
        ar[0] = 1;
        ar[1] = -1;
        ar[2] = 1;
        ar[3] = 1;
        while (true) {
            if (ar[0] == ar[1] && ar[1] == ar[2] && ar[2] == ar[3]) {
                System.out.println("THE BELL IS RINGING");
                break;
            }
            int x, y;
            x = s.nextInt();
            y = s.nextInt();
            ar[x] *= -1;
            ar[y] *= -1;
        }
    }   
}

```
