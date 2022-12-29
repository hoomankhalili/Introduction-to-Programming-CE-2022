```java
int n = a.length;
for (int i = 0; i < n/2; i++) {
    String temp = a[n-i-1];
    a[n-i-1] = a[i];
    a[i] = temp;
}
```
