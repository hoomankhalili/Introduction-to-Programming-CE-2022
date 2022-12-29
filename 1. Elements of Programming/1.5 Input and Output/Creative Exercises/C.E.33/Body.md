**اسیلوسکوپ.** یک برنامه Oscilloscope.java بنویسید تا خروجی یک اسیلوسکوپ را شبیه سازی کند و الگوهای Lissajous را تولید کند. این الگوها به افتخار فیزیکدان فرانسوی، Jules A. Lissajous، که الگوهایی را که هنگام وقوع دو اختلال دوره ای عمود بر یکدیگر به طور همزمان به وجود می آیند، مطالعه کرد. فرض کنید که ورودی ها سینوسی هستند، به طوری که معادلات پارامتری زیر منحنی را توصیف می کند:

$$ x = A_x sin (w_xt + θ_x) $$

$$ y = A_y sin (wyt + θy) $$

$$ A_x, A_y = amplitudes $$

$$ w_x, w_y = angular velocity $$

$$ θ_x, θ_y = phase factors $$

شش پارامتر $A_x, w_x, θ_x, θ_y, w_y, θ_y$ را از command line بگیرید.

برای مثال، اولین تصویر زیر پارامتر های $A_x = A_y = 1, w_x = 2, w_y = 3, θ_x = 20$ درجه, $θ_y = 45$ درجه و تصویر دیگر پارامتر های (1, 1, 5, 3, 30, 45) را دارد.

![oscilloscope](https://introcs.cs.princeton.edu/java/15inout/images/oscilloscope2.png)
![oscilloscope](https://introcs.cs.princeton.edu/java/15inout/images/oscilloscope3.png)
