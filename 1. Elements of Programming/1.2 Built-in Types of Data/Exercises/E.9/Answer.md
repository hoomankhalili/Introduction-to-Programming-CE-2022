````java
public class SumOfTwoDice { 
         public static void main(String[] args){
               int a= (int)(Math.rand() * 6) + 1;
               int b= (int)(Math.rand() * 6) + 1;
               int sum = a+b;
               System.out.print("sum of two random integers is:" + sum);
               }
}
