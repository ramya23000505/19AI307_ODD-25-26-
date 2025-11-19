# Ex.No:3(E) INNER CLASS

## QUESTION:
Write a Java program where the inner class is declared private and accessed through a method in the outer class.

## AIM:
To write a Java program where the inner class is declared private and accessed through a method in the outer class.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create an object of the outer class.
4.	Read an integer input from the user.
5.	Inside the outer class method, create an object of the private inner class.
6.	Pass the user input to the inner class using its setData() method.
7.	The inner class stores the value and returns it using getData().
8.	Display the value retrieved from the private inner class
9.	End the program.


## PROGRAM:

```
Program to implement a InnerClass using Java
Developed by: Ramya R
RegisterNumber: 212223230169
```

## SOURCE CODE:

```
import java.util.Scanner;

public class OuterClass 
{
    private int data;
    private class InnerClass 
    {
        void setData(int value) 
        {
            data = value;
        }
        int getData() 
        {
            return data;
        }
    }
    public void useInnerClass(int value) 
    {
        InnerClass inner = new InnerClass();
        inner.setData(value);
        System.out.println("Data set inside private inner class: " + inner.getData());
    }
    public static void main(String[] args) 
    {
        Scanner scanner = new Scanner(System.in);
        OuterClass outer = new OuterClass();

        int inputValue = scanner.nextInt();
        outer.useInnerClass(inputValue);

        scanner.close();
    }
}
```


## OUTPUT:

<img width="998" height="269" alt="image" src="https://github.com/user-attachments/assets/d38ee818-ea41-480e-adac-58dcc7e1c039" />


## RESULT:
Thus, a java program where the inner class is declared private and accessed through a method in the outer class is written and executed successfully.

