````java
public static GymnasticsScore{
	     public static void main(String[] args){
			 double a=Double.parseDouble(args[0]);
			 double b=Double.parseDouble(args[1]);
			 double c=Double.parseDouble(args[3]);
			 double d=Double.parseDouble(args[4]);
			 double e=Double.parseDouble(args[5]);
			 double f=Double.parseDouble(args[6]);
			 double max=a;
			 if (b>=max)
				 max=b;
			 else if (c>=max)
				 max=c;
			 else if (d>=max)
				 max=d;
			 else if (e>=max)
				 max=e;
			 else if (f>=max)
				 max=f;
			 double min=a;
			 if (b<=min)
				 min=b;
			 else if (c<=min)
				 min=c;
			 else if (d<=min)
				 min=d;
			 else if (e<=min)
				 min=e;
			 else if (f<=min)
				 min=f;
			 double sum=(a+b+c+d+e+f)-(min+max);
			 double ave=sum/4;
			 System.out.print(ave);
		 }
}
