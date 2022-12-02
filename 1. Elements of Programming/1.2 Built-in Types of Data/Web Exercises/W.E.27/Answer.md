````java
public class Discriminant{
         public static void main(String[] args){
         double b=Double.parsedouble(args[0]);
         double c=Double.parseDouble(args[1]);
         double d=Double.parseDouble(args[2]);
         
         double answer=Math.pow(b,Math.pow(2*c,2)) - Math.pow(4*c,3) - Math.pow(4*b,3*d) - Math.pow(27*d,2) + 18*b*c*d;
         System.out.print(answer);
        }
}
