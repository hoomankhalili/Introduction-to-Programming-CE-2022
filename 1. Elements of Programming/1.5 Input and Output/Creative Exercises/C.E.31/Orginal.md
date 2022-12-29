**Spirographs.** Write a program Spirograph.java that takes three command-line arguments R, r, and a and draws the resulting spirograph. A [spirograph](https://en.wikipedia.org/wiki/Spirograph) (technically, an epicycloid) is a curve formed by rolling a circle of radius r around a larger fixed circle or radius R. If the pen offset from the center of the rolling circle is (r+a), then the equation of the resulting curve at time t is given by

$$ x(t) = (R+r)*cos(t) - (r+a)*cos(((R+r)/r)*t) $$

$$ y(t) = (R+r)*sin(t) - (r+a)*sin(((R+r)/r)*t) $$

Such curves were popularized by a best-selling toy that contains discs with gear teeth on the edges and small holes that you could put a pen in to trace spirographs.

For a dramatic 3d effect, draw a circular image, e.g., [earth.gif](https://introcs.cs.princeton.edu/java/15inout/earth.gif) instead of a dot, and show it rotating over time. Here's a picture of the resulting [spirograph](https://introcs.cs.princeton.edu/java/15inout/images/spirograph.png) when R = 180, r = 40, and a = 15.
