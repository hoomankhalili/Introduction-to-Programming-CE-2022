```java
public class MoreDuke {

    public static void main(String[] args) {
        // image width = 130-by-80
        int IMAGES     = 17;                      // images per cartwheel
        int CARTWHEELS = 5;                       // cartwheels per cycle
        int CYCLES     = 100;                     // number of cycles
        int OVERLAP    = 57;                      // overlap between two carthweels
        int WIDTH      = OVERLAP * CARTWHEELS;    // width of the window
        int HEIGHT     = 80;                      // height of the window
        StdDraw.setCanvasSize(WIDTH, HEIGHT);
        StdDraw.setXscale(0, WIDTH);
        StdDraw.setYscale(0, HEIGHT);
        StdDraw.enableDoubleBuffering();

        // main animation loop
        int x = WIDTH * CYCLES;
        for (int t = 0; t < CYCLES; t++) {
            x -= OVERLAP;
            for (int i = 1; i <= IMAGES; i++) {
                StdDraw.clear();
                String filename = "T" + i + ".gif";     // name of ith image
                StdDraw.picture(x % WIDTH, HEIGHT/2.0, filename);
                StdDraw.picture(WIDTH + x % WIDTH, HEIGHT/2.0, filename);
                StdDraw.show();
                StdDraw.pause(100);
            }
            StdDraw.pause(1000);
        }


    }

}
```
