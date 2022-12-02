````java
public class WindChill {
         public static void main(String[] args){
               double t=Double.parseDouble(args[0]);
               double v=Double.parseDouble(args[1]);
               double w=35.74+0.6215*t+(0.4275*t - 35.75)*(Math.pow(v,0.16));
               if (t<50 && 3<v<120)
               System.out.print("Wind chill : " + w);
               else 
               System.out.print("The formula is not valid")
         }
}
