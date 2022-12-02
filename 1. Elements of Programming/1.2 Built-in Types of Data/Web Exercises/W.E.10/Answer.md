```java

public class MainClass {
	    private static String fibWord(int n) {
	        String wordN = "b";
	        String wordN_1 = "a";
	        String temp;

	        for (int i = 2; i <= n; i++) {
	            temp = wordN;
	            wordN += wordN_1;
	            wordN_1 = temp;
	        }

	        return wordN;
	    }

	    public static void main(String[] args) {
	    	System.out.println("Enter the n: ");
	        int n = Integer.parseInt(args[0]);
	        System.out.println(fibWord(n));
	    }
	}
```
