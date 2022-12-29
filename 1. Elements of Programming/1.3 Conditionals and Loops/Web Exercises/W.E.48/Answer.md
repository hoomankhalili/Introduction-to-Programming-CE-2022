```java
public class Main {

    public static void main(String[] args) {
        
        int N = Integer.parseInt(args[0]);
        int quarters = 0;
        int dims = 0;
        int nickels = 0;
        int pennies = 0;

        while (N>=25){
            N = N - 25;
            quarters++;
        }
        while (N>=10){
            N = N - 10;
            dims++;
        }
        while (N>=5){
            N = N - 5;
            nickels++;
        }
        while (N>=1){
            N = N - 1;
            pennies++;
        }
        
        System.out.println("quarter " + quarters);
        System.out.println("dim " + dims);
        System.out.println("nickel " + nickels);
        System.out.println("penny " + pennies);

    }

}
```