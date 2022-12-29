````java
public class Kary
{
    public static void main(String[] args) {
        int i = Integer.parseInt(args[0]);
        int k = Integer.parseInt(args[1]);
         String s="";
         int power = 1;
         while (power <= i/k)
         {
             power *= k;
         }   
         if (k <= 10)
         {
             while (power > 0)
             {
                 int digit = i / power;
                 System.out.print(digit);
                 i -= digit * power;
                 power /= k;
             }
         }
         
         else if (k > 10)
         {   while (i>0) {
        	 
             int q=i%16;
             i/=16;
               switch (q)
             {   
                 case 15: s="F" + s; break;
                 case 14: s="E" + s; break;
                 case 13: s="D" + s; break;
                 case 12: s="C" + s; break;
                 case 11: s="B" + s; break;
                 case 10: s="A" + s; break;
                 case 9: s="9" + s; break;
                 case 8: s="8" + s; break;
                 case 7: s="7" + s; break;
                 case 6: s="6" + s; break;
                 case 5: s="5" + s; break;
                 case 4: s="4" + s; break;
                 case 3: s="3" + s; break;
                 case 2: s="2" + s; break;
                 case 1: s="1" + s; break;
            } //end switch
           } //end while
         } //end else
         System.out.print(s);
	} //end main

} //end class
