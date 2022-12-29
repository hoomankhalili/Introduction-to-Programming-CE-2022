```java
public class DistinctABC {
	public static void main(String[] args) {
		int a = Integer.parseInt(args[0]);
		int b = Integer.parseInt(args[1]);
		int c = Integer.parseInt(args[2]);
		if (a == b && a != c)
			System.out.println(2);	
		if (a != b && b == c)
			System.out.println(2);
		if (a != b && a == c)
			System.out.println(2);
		if (a == b && a == c)
			System.out.println(1);
		if (a != b && a != c && b != c)
			System.out.println(3);
	
		
	}

}
```
