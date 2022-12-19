````java
public class windspeed {
	      public static void main(String[] args){
			  int w=Integer.parseInt(args[0]);
			  switch(w) {
			  case 0<=w<1:
			  System.out.print("0");
			  break;
			  case 1<=w<=3:
			  System.out.print("1");
			  break;
			  case 4<=w<=6:
			  System.out.print("2");
			  break;
			  case 7<=w<=10:
			  System.out.print("3");
			  break;
			  case 11<=w<=16:
			  System.out.print("4");
			  break;
			  case 17<=w<=21:
			  System.out.print("5");
			  break;
			  case 22<=w<=27:
			  System.out.print("6");
			  break;
			  case 28<=w<=33:
			  System.out.print("7");
			  break;
			  case 34<=w<40:
			  System.out.print("8");
			  break;
			  case 41<=w<=47:
			  System.out.print("9");
			  break;
			  case 48<=w<=55:
			  System.out.print("10");
			  break;
			  case 56<=w<=63:
			  System.out.print("11");
			  break;
			  case 63<w:
			  System.out.print("12");
			  break;
			  }
		  }
}
