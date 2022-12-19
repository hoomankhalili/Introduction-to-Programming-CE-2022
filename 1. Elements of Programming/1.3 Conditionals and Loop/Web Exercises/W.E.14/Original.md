What does the following program do?
```java
public static void main(String[] args) {
   int N = Integer.parseInt(args[0]);
   int x = 1;
   while (N >= 1) {
      System.out.println(x);
      x = 2 * x;
      N = N / 2;
   }
}
```
