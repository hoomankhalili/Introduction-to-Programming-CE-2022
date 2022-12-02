```java
public class Divisibility {
	public static void main(String[] args) {
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);
		boolean isDivisable = (a % 7 == 0) && (b % 7 == 0);
		System.out.println(isDivisable);
	}
}
```
