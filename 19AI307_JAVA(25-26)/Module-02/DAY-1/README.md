# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Define a class Car with brand (String), color (String), and year (int). Create 2 different objects of Car  Assign values to attributes. Print the details of both cars.

## AIM:
To Write a program and define a class Car with brand (String), color (String), and year (int). Create 2 different objects of Car  Assign values to attributes. Print the details of both cars.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define class Car with attributes: brand, color, year.
4.	Add method printDetails() to display these attributes.
5.	In main(), create a Scanner object.
6.	Create two Car objects.
7.	Read brand, color, and year for both objects and assign values.
8.	Call printDetails() for both objects to print their details.
9.	End of the program.

   
## PROGRAM:
 ```
/*
Program to implement a Class and Objects using Java
Developed by: RAMYA R
RegisterNumber:  212223230169
*/
```

## SOURCE CODE:

```
import java.util.*;
class Car 
{
    String brand;
    String color;
    int year;

    void printDetails() 
    {
        System.out.println("Brand: "+brand);
        System.out.println("Color: "+ color);
        System.out.println("Year: "+year);
    }
}

class prog {
    public static void main(String[] args)
    {
        Scanner sc = new Scanner(System.in);
        
        Car obj1 = new Car();
        Car obj2 = new Car();
        
        obj1.brand = sc.next();
        obj1.color = sc.next();
        obj1.year = sc.nextInt();
        
        obj2.brand = sc.next();
        obj2.color = sc.next();
        obj2.year = sc.nextInt();
        
        obj1.printDetails();
        obj2.printDetails();
    }
}
```

## OUTPUT:
<img width="683" height="710" alt="image" src="https://github.com/user-attachments/assets/eb2c18b3-a618-4474-89bb-cbb02cd120ea" />

## RESULT:
Thus, the program creates a Car class with attributes and a printDetails method, reads input for two Car objects, assigns their values, prints their details, and ends.
