# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Define a class Car with brand (String), color (String), and year (int). Create 2 different objects of Car  Assign values to attributes. Print the details of both cars.

## AIM:
To Write a program and define a class Car with brand (String), color (String), and year (int). Create 2 different objects of Car  Assign values to attributes. Print the details of both cars.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	





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
## Test Result Table

| Input                    | Expected                                         | Got                                              |
|--------------------------|---------------------------------------------------|---------------------------------------------------|
| Toyota<br>Red<br>2015<br>Honda<br>Blue<br>2018 | Brand: Toyota<br>Color: Red<br>Year: 2015<br>Brand: Honda<br>Color: Blue<br>Year: 2018 | Brand: Toyota<br>Color: Red<br>Year: 2015<br>Brand: Honda<br>Color: Blue<br>Year: 2018 |
| Ford<br>Black<br>2020<br>BMW<br>White<br>2017 | Brand: Ford<br>Color: Black<br>Year: 2020<br>Brand: BMW<br>Color: White<br>Year: 2017 | Brand: Ford<br>Color: Black<br>Year: 2020<br>Brand: BMW<br>Color: White<br>Year: 2017 |
| Tesla<br>White<br>2022<br>Audi<br>Grey<br>2019 | Brand: Tesla<br>Color: White<br>Year: 2022<br>Brand: Audi<br>Color: Grey<br>Year: 2019 | Brand: Tesla<br>Color: White<br>Year: 2022<br>Brand: Audi<br>Color: Grey<br>Year: 2019 |


## RESULT:


