**Oscilloscope.** Write a program Oscilloscope.java to simulate the output of an oscilloscope and produce Lissajous patterns. These patterns are named after the French physicist, Jules A. Lissajous, who studied the patterns that arise when two mutually perpendicular periodic disturbances occur simultaneously. Assume that the inputs are sinusoidal, so tha the following parametric equations describe the curve:

$$ x = A_x sin (w_xt + θ_x) $$

$$ y = A_y sin (wyt + θy) $$

$$ A_x, A_y = amplitudes $$

$$ w_x, w_y = angular velocity $$

$$ θ_x, θ_y = phase factors $$

Take the six parameters $A_x, w_x, θ_x, θ_y, w_y$ and $θ_y$ from the command line.

For example, the first image below has $A_x = A_y = 1, w_x = 2, w_y = 3, θ_x = 20$ degrees, $θ_y = 45$ degrees. The other has parameters (1, 1, 5, 3, 30, 45)

![oscilloscope](https://introcs.cs.princeton.edu/java/15inout/images/oscilloscope2.png)
![oscilloscope](https://introcs.cs.princeton.edu/java/15inout/images/oscilloscope3.png)
