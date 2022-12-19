````java
public class PowersOfK {
	      public static void main(String[] args){
			  int k=Integer.parseInt(args[0]);
			  int i=1;
			  long a=k;
			  while (a<Long.MAX_VALUE){
				  System.out.print(i+" ");
				  System.out.print(a);
                                  i++;
				  a= (long) Math.pow(k,i);
			  }
		 }
}
