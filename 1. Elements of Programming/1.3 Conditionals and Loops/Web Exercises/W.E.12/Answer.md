````java
public class RGBtoHSV {
         public static void main(String[] args){
                 int B=Integer.parseInt(args[0]);
                 int G=Integer.parseInt(args[1]);
                 int R=Integer.parseInt(args[2]);
         
         int max=B;
				 if (G>=max)
					 max=G;
				 else if (R>=max)
					 max=R;
				 int min=B;
				 if (B<=min)
					 min=G;
				 else if (R<=min)
					 min=R;
				 
				 int V=max/255;
				 int H=0;
				 int S=0;
				 if (max>0)
			          S=1-min/max;
				 else if (max=0)
					  S=0;
				 if (G>=B)
					 H=Math.acos((R-1/2*G-1/2*B)/Math.sqrt(R*R+G*G+B*B-R*G-R*B-GB));
				 else 
					 H=360-Math.acos((R-1/2*G-1/2*B)/Math.sqrt(R*R+G*G+B*B-R*G-R*B-G*B));
         
                 System.out.print(H,S,V);
        }
}
