# [Download Java Editor IntelliJ IDEA](https://www.jetbrains.com/idea/download/#section=windows)

```java
import java.util.Scanner;

class HelloWorld {
    public static void main(String[] args) {
        System.out.println("Hello, World!");
        
         System.out.println("Hello, World!");
        
        int intNumber;
        intNumber = 5;
        System.out.println(intNumber);
        
        intNumber = intNumber + 15;
        System.out.println(intNumber);
        
        int intNumber2 = 30;
        System.out.println(intNumber2);
        
        double doubleNumber = 2.5;
        System.out.println(doubleNumber);
        
        System.out.println(5 / 2);
        System.out.println(5. / 2);
        System.out.println(5 / 2.);
        
        String word = "fox";
        System.out.println(word);
        System.out.println("word");
        
        char character = 'f';
        System.out.println(character);
        
        boolean myBool = true;
        boolean myBool2 = false;
        System.out.println(myBool);
        System.out.println(myBool2);
        
        System.out.println(!myBool);
        System.out.println(!myBool2);
        
        //Aritmeticke operacie
        
        /*
        +
        -
        *
        /
        % modulus vrati to zvysok po deleni
        */
        
        System.out.println(intNumber + 2);
        System.out.println(intNumber * 2);
        System.out.println(intNumber % 3); //20 - (20/3)
        
        int i = 1;
        System.out.println(i);
        i = i + 1;
        System.out.println(i);
        
        i += 1;
        System.out.println(i);
        
        // If Else
        /* if(podmienka) {
            co sa stane ak podmienka plati
        }
        */
        
        int number = 4;
        if(number % 2 == 0){
            System.out.println("4 je delitelne 2");
        }
        
        int number2 = 9;
        
        if(number2 % 2 == 0){
            System.out.println("9 je delitelne 2");
        }else {
            System.out.println("9 nie je delitelne 2");
        }
        
        if(number2 % 2 == 0){
            System.out.println("9 je delitelne 2");
        }else if (number2 % 3 == 0) {
            System.out.println("9 je delitelne 3");
        } else {
            System.out.println("9 nie je delitelne 3 ani 2");
        }
        
        // &&- a  || - alebo
        
        int number3 = 6;
        
        if(number3 % 2 == 0  && number3 % 3 == 0){
            System.out.println("6 je delitelne aj 2 aj 3");
        }
        
        if(number % 2 == 0 || number % 3 == 0){
            System.out.println("4 je delitelne 2 alebo 3");
        }
        
        
        //Citanie Inputov
        
        Scanner s = new Scanner(System.in);
        
        System.out.println("Zadaj svoje meno:");
        String name = s.next();
        System.out.println("Hello " + name);
        
        
        System.out.println("Zadaj svoje oblubene zvieratko:");
        String animal = s.next();
        System.out.println("Moje oblubene zvieratko je " + animal);
        
        System.out.println("Zadaj svoj vek: ");
        int age = s.nextInt();
        System.out.println("Moj vek je " + age);
        
        System.out.println("Zadaj svoju vysku: ");
        double height = s.nextDouble();
        System.out.println("Moj vyska je " + height);
        
        //loop
        // for loop
        /* for(inicializacia; podmienka ; update){
            telo
        }
        */
        
        for(int j = 1; j <= 15 ; j++){
            System.out.println(j);
        }
        
        //ako mozem vytlacit parne cisla od 0 do 20
        for(int k = 0; k <= 20; k++ ){
            if(k % 2 ==0 ){
                System.out.println(k);
            }
        }
        
        //sucet parnych cisel od 0 do 20
        int sum = 0;
        for(int k = 0; k <= 10; k += 2){
                sum += k;
        }
        System.out.println(sum);
        
        //while
        int a = 0;
        int sum2 = 0;   
        while( a <= 5){
            sum2 += a;
            a++;
        }
        
        System.out.println(sum2);
        
        //do while
        int num = 1;
        do {
            System.out.println("do while");
        } while (num < 1);
        
        while(num < 1){
            System.out.println("while");
        };
        
        int sum3 = 0;
        int input = 0;
        do{
            input = s.nextInt();
            sum3 += input;
        }while(input != 0);
       
       System.out.println(sum3);
       
       //uhadni cislo
        
       int cislo = 8;
       int tip = 0;
       System.out.println("Hadaj cele cislo od 0 do 10.");
       
       while(cislo != tip){
           tip = s.nextInt();
           if(tip < cislo){
               System.out.println("Skus tipnut vacsie cislo");
           } else if (tip > cislo){
               System.out.println("Skus tipnut mensie cislo");
           } else {
               System.out.println("Uhadol si!");
           }
       };
       
       //priemer suctu kazdeho 5 cisla od 0 do 100
       sum = 0;
       double count = 0.;
        for(int k = 0; k <= 100; k += 3){
                sum += k;
                count++;
        }
        
        double priemer = sum / count;
        System.out.println(priemer);
       
        
    }
}
```