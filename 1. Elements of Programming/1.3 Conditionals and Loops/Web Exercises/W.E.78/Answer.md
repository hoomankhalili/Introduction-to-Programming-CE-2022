```java
public class Main {

    public static void main(String[] args) {

        double weight = Double.parseDouble(args[0]);
        double height = Double.parseDouble(args[1]);

        double BMI = weight / (height * height);

        if (BMI < 15) {
            System.out.println("Starvation");
        } else if (BMI < 17.5) {
            System.out.println("Anorexic");
        } else if (BMI < 18.5) {
            System.out.println("Underweight");
        } else if (BMI >= 18.5 && BMI < 25) {
            System.out.println("Ideal");
        } else if (BMI >= 25 && BMI < 30) {
            System.out.println("Overweight");
        } else if (BMI >= 30 && BMI < 40) {
            System.out.println("Obese");
        } else if (BMI >= 40) {
            System.out.println("Morbidly Obese");
        }

    }

}
```