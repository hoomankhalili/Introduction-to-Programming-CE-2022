```java
public class Main {

    public static void main(String[] args) {

        int windSpeed = Integer.parseInt(args[0]);

        if (windSpeed < 74) {
          System.out.println("Not hurricane");
        } else if (windSpeed < 96) {
          System.out.println("Category 1 hurricane");
        } else if (windSpeed < 111) {
          System.out.println("Category 2 hurricane");
        } else if (windSpeed < 131) {
          System.out.println("Category 3 hurricane");
        } else if (windSpeed < 155) {
          System.out.println("Category 4 hurricane");
        } else {
          System.out.println("Category 5 hurricane");
        }
        
    }

}
```