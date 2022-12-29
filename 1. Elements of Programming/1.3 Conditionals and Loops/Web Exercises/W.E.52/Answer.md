```java
public class Main {

    public static void main(String[] args) {

        int N = 5;

        for (int i=1; i<N; i++) {

            for (int j=N; j>0; j--) {
                if (j <= i) {
                    System.out.print(" * ");
                } else {
                    System.out.print(" . ");
                }

            }
            for (int j=1; j<N; j++) {
                if (j < i) {
                    System.out.print(" * ");
                } else {
                    System.out.print(" . ");
                }

            }

            System.out.println();
        }
        for (int i=0; i<N; i++) {
            for (int j=1; j<N; j++) {
                if (j <= i) {
                    System.out.print(" . ");
                } else {
                    System.out.print(" * ");
                }

            }
            for (int j=N; j>0; j--) {
                if (j <= i) {
                    System.out.print(" . ");
                } else {
                    System.out.print(" * ");
                }

            }
            System.out.println();
        }

    }
    
}
```
