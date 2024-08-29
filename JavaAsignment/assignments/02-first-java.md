# [Video Link](https://youtu.be/TAtrPoaJ7gc)

## Write Java programs for the following:

1. Write a program to print whether a number is even or odd, also take
input from the user.
## answer)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.print("Enter the numbers:");
        int a=in.nextInt();
        if(a%2==0){
            System.out.println("The number is even" + " " +a);
        }
        else{
            System.out.println("The number is odd" + " " + a);
        }
        
    }

}

2. Take name as input and print a greeting message for that particular name.
## answer)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.print("Enter the name:");
        String name=in.nextLine();
        System.out.println("Dear" + " " + name + " " +  "greetings in [native language] and in the universal language of friendship. May our connection transcend borders and boundaries, just as the Voyager spacecraft carries greetings from humanity to the cosmos");
        
    }

}

3. Write a program to input principal, time, and rate (P, T, R) from the user and
find Simple Interest.
## answer)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.print("Enter the P:");
        float P=in.nextFloat();
        System.out.print("Enter the T:");
        float T=in.nextFloat();
        System.out.print("Enter the R:");
        float R=in.nextFloat();
        float ans=P*T*R;
        System.out.println("The simple Interest:" + ans);
        
    }

}

4. Take in two numbers and an operator (+, -, *, /) and calculate the value.
(Use if conditions)
## answer)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        int ans=0;
       while(true){
           char op=in.next().trim().charAt(0);
           if(op=='+'||op=='-'||op=='*'||op=='/'){
               int num1=in.nextInt();
               int num2=in.nextInt();
               if(op=='+'){
                   System.out.println("The sum is:" + (num1+num2));
               }
               if(op=='-'){
                   System.out.println("The sub is:" + (num1-num2));
               }
               if(op=='*'){
                   System.out.println("The mul is:" + (num1*num2));
               }
               if(op=='/'){
                   System.out.println("The div is:" + (num1/num2));
               }


           }
           else if(op=='x'||op=='X'){
               break;
           }
           else{
               System.out.println("Invalid input");
           }
           System.out.println(ans);
       }


    }

}

5. Take 2 numbers as input and print the largest number.
## answer)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.println("Enter two number:");
        int a=in.nextInt();
        int b=in.nextInt();
        if(a>b){
            System.out.println("A is larger number " + a);
        }
        else{
            System.out.println("B is Larger " + b);
        }
    }
}


6. Input currency in rupees and output in USD.
## answer)

import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.println("Enter currency in rupees:");
        float INR=in.nextFloat();
        double USD=INR/83.96f;
        System.out.print("The USD is:" + USD);
    }
}

7. To calculate Fibonacci Series up to n numbers.
## answer)
public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.println("Enter the number:");
       int n=in.nextInt();
       int p=0;
       int i=1;
       int count=2;
       while (count<=n){
           int temp=i;
           i=i+p;
           p=temp;
           count++;
       }
        System.out.println(i);
    }
}

8. To find out whether the given String is Palindrome or not.
## answer)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in=new Scanner(System.in);
        System.out.println("Enter the String:");
        String str=in.next();
        System.out.println(isPalindrom(str));
    }
    static boolean isPalindrom(String str) {

        str = str.toLowerCase();
        for (int i = 0; i <=str.length() / 2; i++) {
            char start = str.charAt(i);
            char end = str.charAt(str.length() - 1 - i);
            if (start != end) {
                return false;
            }
        }
        return true;

    }
}


9. To find Armstrong Number between two given number.
## ans)
import java.util.Scanner;

public class Revision {
    public static void main(String[] args) {
        Scanner in = new Scanner(System.in);
        int a=in.nextInt();
        int original=a;
        int ans=0;
        while(a>0){
            int rem=a%10;
            int cube=rem*rem*rem;
            ans=ans+cube;
            a/=10;
        }
        if(original==ans){
            System.out.println("Yes! it is AramStrong");
        }
        else{
            System.out.println("Yes! it is  not AramStrong");
        }

    }
}


