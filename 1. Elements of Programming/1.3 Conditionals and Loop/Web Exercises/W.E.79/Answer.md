```java
public class Main {

	public static void main(String[] args) {
	
  	double d = Double.parseDouble(args[0]);
	double v = Double.parseDouble(args[1]);
	double rho = Double.parseDouble(args[2]);
	double mu = Double.parseDouble(args[3]);
	double Reynold = (d * v * rho) / mu;
	if (Reynold < 2000) {
		System.out.println("Laminar flow");
	}
	else {
		if(Reynold < 4000){
			System.out.println("Transient flow");
		}
			else {
				System.out.println("Turbulent flow");
			}
		}
	}
}
```
