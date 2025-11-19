# Ex.No:3(b) POLYMORPHISM

## QUESTION:
Write a Java program to create a class Vehicle with a method called speedUp(). Create two subclasses Car and Bicycle. Override the speedUp() method in each subclass to increase the vehicle's speed differently.

## AIM:
To write a Java program to create a class with a method using Polymorphism.


## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define a Vehicle class with a speedUp() method and a speed variable initialized to 0.
4.	Create two subclasses, Car and Bicycle, and override the speedUp() method so that each increases speed differently.
5.	In the main() method, read the vehicle type (car/bicycle) and the increment value from the user.
6.	Based on the input type, create the appropriate object: Car or Bicycle; if type is invalid, display an error and stop.
7.	Call the speedUp() method on the selected object to increase and display the new speed.
8.	End the program.


## PROGRAM:

```
Program to implement a Polymorphism using Java
Developed by: Sathyaa R
RegisterNumber: 212223100052
```

## SOURCE CODE:

```
import java.util.Scanner;

class Vehicle 
{
    protected int speed = 0;
    void speedUp(int increment) 
    {
        speed += increment;
        System.out.println("Vehicle speed increased to: " + speed + " km/h");
    }
}

class Car extends Vehicle 
{
    @Override
    void speedUp(int increment) 
    {
        speed += increment * 2;
        System.out.println("Car speed increased to: " + speed + " km/h");
    }
}

class Bicycle extends Vehicle 
{
    @Override
    void speedUp(int increment) 
    {
        speed += increment; 
        System.out.println("Bicycle speed increased to: " + speed + " km/h");
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        String type = sc.nextLine().toLowerCase();
        int increment = sc.nextInt();
        Vehicle v;

        if (type.equals("car")) 
        {
            v = new Car();
        } 
        else if (type.equals("bicycle")) 
        {
            v = new Bicycle();
        } 
        else 
        {
            System.out.println("Invalid vehicle type");
            sc.close();
            return;
        }
        v.speedUp(increment);
        sc.close();
    }
}
```


## OUTPUT:

<img width="915" height="339" alt="image" src="https://github.com/user-attachments/assets/03942f12-1043-4709-b17c-f43a76b45318" />


## RESULT:
Thus, the program to write a Java program to create a class with a method using Polymorphism is written and executed successfully.

