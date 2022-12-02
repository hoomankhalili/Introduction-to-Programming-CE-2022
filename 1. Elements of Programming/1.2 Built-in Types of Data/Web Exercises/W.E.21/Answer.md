````java
public class HorizontalCoordinates{         
          public static void main(String[] args){
                   double δ=Double.parseDouble(args[0]);
                   double φ=Double.parseDouble(args[1]);
                   double H=Double.parseDouble(args[2]);
                     
                   double Altitude=Math.asin(Math.sin(φ) * Math.sin(δ) + Math.cos(φ) * Math.cos(δ) * Math.cos(H));
                   double Azimuth=Math.acos((Math.cos(φ) * Math.sin(δ) - Math.sin(φ) * Math.cos(δ) * Math.cos(H)) / Math.cos(Altitude));
                   System.out.print(Azimuth);
          }
}
