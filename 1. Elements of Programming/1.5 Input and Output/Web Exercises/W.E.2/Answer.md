```java
public class Answer {
  public static void main(String[] args) {
    Scanner s = new Scanner(System.in);
    double mean = 0;
    double count = 0;
    while (true) {
      int inp = s.nextInt();
      if (inp == 999999) break;
      mean += inp;
      count++;
    }
    System.out.println(mean / count);
  }
}
```
