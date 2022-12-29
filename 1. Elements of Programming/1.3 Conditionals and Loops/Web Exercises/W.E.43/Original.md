What is the value of s after executing the following code?
```java
int M = 987654321;
String s = "";
while (M != 0) {
   int digit = M % 10;
   s = s + digit;
   M = M / 10;
}
```