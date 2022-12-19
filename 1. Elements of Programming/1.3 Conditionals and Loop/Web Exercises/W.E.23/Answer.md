```java
public class Main {

    public static void main(String[] args) {

        int A = Integer.parseInt(args[0]);
        int B = Integer.parseInt(args[1]);
        int C = Integer.parseInt(args[2]);
        int D = Integer.parseInt(args[3]);
        int E = Integer.parseInt(args[4]);

        double W = 250.0/3 * (((double) A / B) - 0.3);
        double X = 25.0/6 * (((double) C / B) - 3);
        double Y = 1000.0/3 * ((double) D / B);
        double Z = 1250.0/3 * (0.095 - ((double) E / B));

        double answer = W + X + Y + Z;

        System.out.println("quarterback rating is: " + answer);

    }

}
```