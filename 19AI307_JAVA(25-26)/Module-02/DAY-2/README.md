# Ex.No:2(B) METHODS

## QUESTION:
Write a method boolean isEven  (int num) without using % operator that returns true if the number is even.

## AIM:
To write a method boolean isEven  (int num) without using % operator that returns true if the number is even.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Take an integer num as input.
4.	Perform a bitwise AND operation between num and 1.
5.	If the result is 0, then the number is even.
6.	Otherwise, the number is odd.
7.	Return true for even, false for odd.
8.	End of the program.

## PROGRAM:
 ```
/*
Program to implement a Methods using Java
Developed by: RAMYA R 
RegisterNumber:  212223230169
*/
```

## SOURCE CODE:

```
import java.util.*;

class prog
{
    static boolean isEven(int num)
    {
        return (num & 1) == 0;
    }
    public static void main(String[] argv)
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        System.out.println(isEven(n));
    }
```

## OUTPUT:

<img width="435" height="259" alt="image" src="https://github.com/user-attachments/assets/5ad0310f-a43b-4704-8cd4-5a96fe2353f0" />


## RESULT:
Thus, the result is that the number is identified as even when (num & 1) == 0, otherwise it is odd.
