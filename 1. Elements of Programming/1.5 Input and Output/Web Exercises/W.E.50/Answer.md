```java
import java.io.File;
import java.io.PrintWriter;
import java.util.Scanner;

public class DeleteX {
    public static void main(String[] args) {
        String filePath = args[0];
        String input = null;
        String result = "";
        Scanner sc = new Scanner(new File(filePath));
        StringBuffer sb = new StringBuffer();
        while (sc.hasNextLine()) {
            input = sc.nextLine();
            sb.append(input);
        }
        result = sb.toString();
        //Replacing the word with desired one
        result = result.replaceAll("\bx\b", "");
        PrintWriter writer = new PrintWriter(new File(args[1]));
        writer.append(result);
        writer.flush();
    }
}

```
