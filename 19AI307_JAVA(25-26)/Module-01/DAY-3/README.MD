# Ex.No:1(C) LOOPING STATEMENT

## QUESTION:
Write a Java program to reverse a number using a while loop.

## AIM:
To write a Java program to reverse a number using a while loop.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Read an integer number from the user and store it in num.
4.	Initialize a variable reversed to 0.
5.	Repeat while num > 0:
   a. Extract the last digit using digit = num % 10.
  	b. Update reversed number: reversed = reversed * 10 + digit.
  	c. Remove the last digit from num using num = num / 10.
6. Display the value of reversed
7. End the program.


## PROGRAM:

```
Program to implement a Looping Statement using Java
Developed by: Ramya R
RegisterNumber: 212223230169
```

## SOURCE CODE:

```
import java.util.Scanner;

public class ReverseNumber 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        int num = sc.nextInt();
        int reversed = 0;

        while (num > 0) 
        {
            int digit = num % 10;
            reversed = reversed * 10 + digit;
            num /= 10;
        }

        System.out.println("Reversed number: " + reversed);
    }
}
```

## OUTPUT:

<img width="642" height="270" alt="image" src="https://github.com/user-attachments/assets/10b2abc4-f704-4309-82f6-26e546997ae2" />


## RESULT:
Thus, the program to write a Java program to reverse a number using a while loop is written and executed successfully.

