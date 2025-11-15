# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class that uses a constructor to count the number of objects created.

## AIM:
To write a class that uses a constructor to count the number of objects created.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class with a static variable to count objects.
4.	Define a constructor that increments the static counter whenever an object is created.
5.	In main(), read the number of objects to be created (n).
6.	Use a loop to create n objects of the class.
7.	After the loop, print the value of the static counter.
8.	End the program.

## PROGRAM:
 ```
/*
Program to implement a Variable scope and Constructor using Java
Developed by: RAMYA R 
RegisterNumber:  212223230169
*/
```

## SOURCE CODE:

```
import java.util.*;
public class Myclass
{
    static int cnt=0;
    Myclass()
    {
        cnt++;
    }
    public static void main(String[] argv)
    {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        for(int i=0;i<n;i++)
        {
           new Myclass();   
        }
        
        System.out.println("Number of objects created: "+cnt);
    }
    
}
```

## OUTPUT:
<img width="836" height="347" alt="image" src="https://github.com/user-attachments/assets/e77163bc-1e48-434b-8091-21a9d54b650c" />


## RESULT:
Thus, the constructor increments the counter for every object created, and the program displays the total number of objects created as given in the input.
