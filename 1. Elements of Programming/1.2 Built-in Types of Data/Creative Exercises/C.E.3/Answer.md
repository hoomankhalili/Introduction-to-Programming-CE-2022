````java
public class DayOfWeek {
         public static void main(String[] args){
                int m=Integer.parseInt(args[0]);
                int d=Integer.parseInt(args[1]);
                int y=Integer.parseInt(args[2]);
                
                int y0=2000 - (14-2) / 12;
                int x =y0 + y0 / 4 -y0 / 100 + y0 / 400;
                int m0=2 + 12 * ((14-2) / 12) - 2;
                int d0= (14 + x + (31 * m0) / 12) % 7;
                System.out.print(d0);
         }
}
