برنامه جاوا زیر را در نظر بگیرید.
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
فرض کنید فایل input.txt شامل اعداد صحیح 1 و 1 باشد. دستور زیر چه کاری انجام می دهد؟
```
java Mystery < input.txt | java Mystery | java Mystery | java Mystery
```