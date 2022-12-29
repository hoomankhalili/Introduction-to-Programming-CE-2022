```java
public class Main {

    public static void main(String[] args) {

        int a = Integer.parseInt(args[0]);
        int b = Integer.parseInt(args[1]);
        int c = Integer.parseInt(args[2]);
        int d = Integer.parseInt(args[3]);
        int e = Integer.parseInt(args[4]);
        int temp = 0;

        for (int i=0; i<2; i++) {
            if (a < b) {
                temp = a;
                a = b;
                b = temp;
            }
            if (b < c) {
                temp = b;
                b = c;
                c = temp;
            }
            if (c < d) {
                temp = c;
                c = d;
                d = temp;
            }
            if (d < e) {
                temp = d;
                d = e;
                e = temp;
            }

        }

        System.out.println(c);

    }

}

```
