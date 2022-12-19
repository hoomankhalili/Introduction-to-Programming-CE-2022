```java
public class Season {
    public static void main(String[] args) {
        int M = Integer.parseInt(args[0]);
        int D = Integer.parseInt(args[1]);
        if (M == 1) {
            System.out.println("Winter");
        } else if (M == 2) {
            System.out.println("Winter");
        } else if (M == 3) {
            if (D <= 20) System.out.println("Winter");
            else System.out.println("Spring");
        } else if (M == 4) {
            System.out.println("Spring");
        } else if (M == 5) {
            System.out.println("Spring");
        } else if (M == 6) {
            if (D <= 20) System.out.println("Spring");
            else System.out.println("Summer");
        } else if (M == 7) {
            System.out.println("Summer");
        } else if (M == 8) {
            System.out.println("Summer");
        } else if (M == 9) {
            if (D <= 22) System.out.println("Summer");
            else System.out.println("Fall");
        } else if (M == 10) {
            System.out.println("Fall");
        } else if (M == 11) {
            System.out.println("Fall");
        } else if (M == 12) {
            if (D <= 21) System.out.println("Fall");
            else System.out.println("Winter");
        }
    }
}
```
