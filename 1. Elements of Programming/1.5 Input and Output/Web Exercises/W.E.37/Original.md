Consider the following program.
```java
public class Mystery {
   public static void main(String[] args) {
      int N = Integer.parseInt(args[0]);
      int[] a = new int[M];

      while(!StdIn.isEmpty()) {
         int num = StdIn.readInt();
         a[num]++;
      }

      for (int i = 0; i < M; i++)
         for (int j = 0; j < a[i]; j++)
            System.out.print(i + " ");
      System.out.println();
   }
}
```
Suppose the file input.txt contains the following integers:
```
8 8 3 5 1 7 0 9 2 6 9 7 4 0 5 3 9 3 7 6
```
What is the contents of the array a after running the following command
```
java Mystery 10 < input.txt
```
