**Quarterback rating.** To compare NFL quarterbacks, the NFL devised a the [quarterback rating](http://www.mathnotes.com/aw_quarterback.html) formula based on the quarterbacks number of completed passes (A), pass attempts (B), passing yards (C), touchdown passes (D), and interception (E) as follows:      
       
a.Completion ratio: W = 250/3 * ((A / B) - 0.3).      
b.Yards per pass: X = 25/6 * ((C / B) - 3).     
c.Touchdown ratio: Y = 1000/3 * (D / B).        
d.Interception ratio: Z = 1250/3 * (0.095 - (E / B)).      
       
The quarterback rating is computed by summing up the above four quantities, but rounding up or down each value so that it is at least 0 and and at most 475/12. Write a program QuarterbackRating.java that takes five command line inputs A, B, C, D, and E, and prints the quarterback rating. Use your program to compute Steve Young's 1994 record-setting season (112.8) in which he completed 324 of 461 passes for 3,969 yards, and threw 35 touchdowns and 10 interceptions. As of 2014, the all-time single-season record is 122.5 by Aaron Rodgers in 2011.
