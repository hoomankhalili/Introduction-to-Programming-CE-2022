مقدار s بعد از اجرای کد زیر چیست؟
```java
int M = 987654321;
String s = "";
while (M != 0) {
   int digit = M % 10;
   s = s + digit;
   M = M / 10;
}
```
