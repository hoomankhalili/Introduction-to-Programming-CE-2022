Consider the following Java program.
```java
public class Mystery {
   public static void main(String[] args) {
      int i = StdIn.readInt();
      int j = StdIn.readInt();
      System.out.println((i-1));
      System.out.println((j*i));
   }
}
```
Suppose that the file input.txt contains
```
5 1
```
What does the following command do?
```java Mystery < input.txt```
