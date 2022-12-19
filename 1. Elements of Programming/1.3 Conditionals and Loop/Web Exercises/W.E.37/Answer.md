````java
public class Binary2 {

	public static void main(String[] args) {
		int i =20;
        int k = 2;
         
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
         
   } //end main
} //end class
