```java
public class Main {

    public static void main(String[] args) {

        boolean cboy = true;
        boolean cgirl = true;
        int iter = 100000;
        int random = 0;
        int count = 0;
        int totalcount = 0;
        int two = 0;
        int three = 0;
        int four = 0;
        int higherThanFive = 0;

        for (int i=0; i<=iter; i++) {

            count = 0;
            cboy = true;
            cgirl = true;
            while (cboy || cgirl) {
                random = (int)(Math.random()*2 + 1);
                if (random == 1) {
                    cboy = false;
                } else if (random == 2){
                    cgirl = false;
                }
                count++;
            }
            totalcount += count;

            if (count == 2) {
                two++;
            } else if (count == 3) {
                three++;
            } else if (count == 4) {
                four++;
            } else if (count >= 5) {
                higherThanFive++;
            }

        }

        System.out.println("2: " + two);
        System.out.println("3: " + three);
        System.out.println("4: " + four);
        System.out.println("5<: " + higherThanFive);
        System.out.println((double) totalcount / iter);
        
    }

}
```