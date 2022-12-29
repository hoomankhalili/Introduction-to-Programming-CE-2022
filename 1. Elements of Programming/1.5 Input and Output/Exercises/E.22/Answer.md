```java
import java.awt.Font;

public class Banner {

    public static void main(String[] args) {

        String s = args[0];
        int speed = Integer.parseInt(args[1]);

        Font font = new Font("Arial", Font.BOLD + Font.ITALIC, 50);

        StdDraw.setFont(font);
        StdDraw.setPenColor(StdDraw.BLACK);
        StdDraw.enableDoubleBuffering();


        for (double i = 0.0; true; i += 0.01) {
            
            StdDraw.clear(StdDraw.BOOK_LIGHT_BLUE);
            StdDraw.text((i % 1.0),       0.5, s);
            StdDraw.text((i % 1.0) - 1.0, 0.5, s);
            StdDraw.text((i % 1.0) + 1.0, 0.5, s);
            StdDraw.pause(speed);
            StdDraw.show();
        }

    }

}
```
