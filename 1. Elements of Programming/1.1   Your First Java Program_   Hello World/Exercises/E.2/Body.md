برنامه UseArgument.java را طوری تغییر دهید تا برنامه ای به نام UseThree.java بسازید که سه نام را بگیرد و جمله ای مناسب با نام ها در عکس ترتیب داده شده در خروجی چاپ نماید. به نحوی که برای مثال ورودی "java UseThree Alice Bob Carol" خروجی "Hi Carol, Bob, and Alice." را نتیجه دهد.
```java
public class UseArgument {

    public static void main(String[] args) {
        System.out.print("Hi, ");
        System.out.print(args[0]);
        System.out.println(". How are you?");
    }

}
```
