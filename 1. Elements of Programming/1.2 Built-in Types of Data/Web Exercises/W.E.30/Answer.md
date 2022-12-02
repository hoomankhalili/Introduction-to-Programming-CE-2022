````java
public class CarLoan {
          public static void main(String[] args){
                  double R=Double.parseDouble(args[0]);
                  double P=Double.parseDouble(args[1]);
                  double Y=Double.parseDouble(args[2]);
                  
                  double n=12 * Y;
                  double r=(R / 100) / 12;
                  
                  double payment=(P * r) / (1 - (Math.pow((1+r),(-n)));
                  System.out.print("Monthly payments: " + payment);
           }
}
