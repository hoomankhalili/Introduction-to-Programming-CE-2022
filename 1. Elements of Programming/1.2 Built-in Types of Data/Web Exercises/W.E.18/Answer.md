````java
public class Ordered{
         public static void main(String[] srgs){
                   int x=Integer.parseInt(args[0]);
                   int y=Integer.parseInt(args[1]);
                   int z=Integer.parseInt(args[2]);
                   boolian b;
                   if (x<y && y<z)
                   b=true;
                   else if (x>y && y>z)
                   b=true;
                   else 
                   b=false;
                   System.out.print(b);
                   
         }
}
