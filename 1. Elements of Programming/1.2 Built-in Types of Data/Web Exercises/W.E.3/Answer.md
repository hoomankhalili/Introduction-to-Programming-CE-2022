````java
public class RGBtoYIQ {
         public static void main(String[] args){
                 int B=Integer.parseInt(args[0]);
                 int G=Integer.parseInt(args[1]);
                 int R=Integer.parseInt(args[2]);
         
                 double Y=0.30*R+0.59*G+0.11*B;
                 double I=-0.27*(B-Y)+0.74*(R-Y);
                 double Q=0.41*(B-Y)+0.48*(R-Y);
         
                 System.out.print(Y,I,Q);
        }
}





public class YIQtoRGB {
         public static void main(string[] args){
                 double Y=Double.parseDouble(args[0]);
                 double I=Double.parseDouble(args[1]);  
                 double Q=Double.parseDouble(args[2]);
                 
                 double R=Y+0.9469*I+0.6236*Q;
                 double G=Y-0.2748*I-0.6357*Q;
                 double B=Y-1.1*I+1.7*Q;
                 
                 System.out.print(R,G,B);
        }
}
