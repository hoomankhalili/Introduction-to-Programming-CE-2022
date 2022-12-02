```java
import java.lang.Math;

public class SumOfSines {

	public static void main(String[] args) {
        double t = Double.parseDouble(args[0]);;
        double rad = Math.toRadians(t);
        System.out.println(Math.sin(2 * rad) + Math.sin(3 * rad));
		

	}

}

```
