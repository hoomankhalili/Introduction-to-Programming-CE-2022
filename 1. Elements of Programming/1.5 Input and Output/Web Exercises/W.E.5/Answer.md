```java
public class Head {
  public static void main(String[] args) {
      BufferedReader reader;
      reader = new BufferedReader(new FileReader("sample.txt"));
      Scanner s = new Scanner(System.in);
      int n = s.nextInt();
      for (int i = 0; i < n; i++) {
        String line = reader.readLine();
        if (line != null) System.out.println(line);
        else break;
      reader.close();
  }
}
```
```java
import org.apache.commons.io.input.ReversedLinesFileReader;
public class Tail {
  public static void main(String[] args) {

      File file = new File("D:\\file_name.xml");
      ReversedLinesFileReader object = new ReversedLinesFileReader(file);
      Scanner s = new Scanner(System.in);
      int n = s.nextInt();
      for (int i = 0; i < n; i++) {
        String line = object.readLine();
        if (line != null) System.out.println(line);
        else break;
      reader.close();
  }
}
```
