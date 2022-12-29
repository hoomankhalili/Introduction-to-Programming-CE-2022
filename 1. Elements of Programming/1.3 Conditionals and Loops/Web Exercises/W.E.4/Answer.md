```java
public class Main {

    public static void main(String[] args) {

        int a = Integer.parseInt(args[0]);
        int b = Integer.parseInt(args[1]);
        int c = Integer.parseInt(args[2]);
        int d = Integer.parseInt(args[3]);
        int e = Integer.parseInt(args[4]);
        int temp = 0;
        
        if(b < a){
        tmp = a;
        a = b;
        b = tmp;
        }
        
        if(d < c){
        tmp = c;
        c = d;
        d = tmp;
        }
        
        if(c < a){
        tmp = b;
        b = d;
        d = tmp; 
        c = a;
        }
        
        a = e;
        
        if(b < a){
        tmp = a;
        a = b;
        b = tmp;
        }
        
        if(a < c){
        tmp = b;
        b = d;
        d = tmp; 
        a = c;
        }
        
        if(d < a){
        return d;
        }
        else{
        return a;
        }
} 
```
