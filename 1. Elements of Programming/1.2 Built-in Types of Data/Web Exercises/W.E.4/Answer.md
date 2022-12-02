```java
import java.util.Arrays;

public class CMYKtoRGB {
    public static void main(String[] args) {
        int[] rgb = cmykToRgb(
            Integer.parseInt(args[0]),
            Integer.parseInt(args[1]),
            Integer.parseInt(args[2]),
            Integer.parseInt(args[3])
        );

        System.out.println(Arrays.toString(rgb));
    }

    private static int[] cmykToRgb(int c, int m, int y, int k) {
        int r = 255 * (1 - c) * (1 - k);
        int g = 255 * (1 - m) * (1 - k);
        int b = 255 * (1 - y) * (1 - k);
        int[] rgb = new int[]{ r, g, b };

        return rgb;
    }
}
```
