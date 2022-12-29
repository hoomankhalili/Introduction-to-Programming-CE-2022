Consider the following Java program.
```java
public class Mystery {
   public static void main(String[] args) {
      int i = StdIn.readInt();
      int j = StdIn.readInt();
      int k = i + j;
      System.out.println(j);
      System.out.println(k);
   }
}
```
Suppose that the file input.txt contains the integers 1 and 1. What does the following command do?
```
java Mystery < input.txt | java Mystery | java Mystery | java Mystery
```
