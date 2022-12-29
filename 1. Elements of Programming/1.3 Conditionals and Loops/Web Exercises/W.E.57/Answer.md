````java
public class kickboxing{
	     public static void main(String[] args){
			 int a=Integer.parseInt(args[0]);
			 switch(a){
			 case 0<=a<112:
			 System.out.print("Flyweight");
			 break;
			 case 112<=a<115:
			 System.out.print("Super flyweight");
			 break;
			 case 115<=a<118:
			 System.out.print("Bantamweight");
			 break;
			 case 118<=a<122:
			 System.out.print("Super bantamweight");
			 break;
			 case 122<=a<126:
			 System.out.print("Featherweight");
			 break;
			 case 126<=a<130:
			 System.out.print("Super featherweight");
			 break;
			 case 130<=a<135:
			 System.out.print("Lightweight");
			 break;
			 case 135<=a<140:
			 System.out.print("Super lightweight");
			 break;
			 case 140<=a<147:
			 System.out.print("Welterweight");
			 break;
			 case 147<=a<154:
			 System.out.print("Super welterweight");
			 break;
			 case 154<=a<160:
			 System.out.print("Middleweight");
			 break;
			 case 160<=a<167:
			 System.out.print("Super middleweight");
			 break;
			 case 167<=a<175:
			 System.out.print("Light heavyweight");
			 break;
			 case 175<=a<183:
			 System.out.print("Super light heavyweight");
			 break;
			 case 183<=a<190:
			 System.out.print("Cruiserweight");
			 break;
			 case 190<=a<220:
			 System.out.print("Heavyweight");
			 break;
			 case 220<=a:
			 System.out.print("Super heavyweight");
			 break;
			 }
		 }
}
