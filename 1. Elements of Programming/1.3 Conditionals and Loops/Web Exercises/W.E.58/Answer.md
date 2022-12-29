```java
public class Main {

    public static void main(String[] args) {

        int N = Integer.parseInt(args[0]);
        
        long a5=0;
        long b5=0;
        long c5=0;
        long d5=0;
        long e5=0;

        for (long a=1; a<=N; a++) {
            a5 = a*a*a*a*a;
            for (long b=a; b<=N; b++) {
                b5 = b*b*b*b*b;
                for (long c=b; c<=N; c++) {
                    c5 = c*c*c*c*c;
                    for (long d=c; d<=N; d++) {
                        d5 = d*d*d*d*d;
                        for (long e=1; e<=N; e++) {
                            e5 = e*e*e*e*e;
                            if (a5 + b5 + c5 + d5 == e5) {
                                System.out.println(a + " , " + b + " , " + c + " , " + d + " , " + e);
                            }
                        }
                    }
                }
            }
        }

    }

}
```