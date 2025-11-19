# Ex.No:3(A) INHERITANCE AND AGGREGATION

## QUESTION:
Create a Super class Person with fields name and age. Create a subclass Student that inherits from Person and adds a field marks (integer). Implement a method in Student called calculateGrade() which returns the grade

## AIM:
To write a java program to create a Super class with fields using inheritance.

## ALGORITHM :

1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Define the Person class with fields name and age, then create the Student subclass with marks.
4.	Implement the calculateGrade() method in Student to return the grade based on marks.
5.	Implement the display() method to print name, age, marks, and grade.
6.	In main(), read name, age, and marks from the user.
7.	Create a Student object and assign the input values to it.
8.	Call the display() method to show the student's details and grade.
9.	End the program.


## PROGRAM:

```
Program to implement a Inheritance and Aggregation using Java
Developed by: Ramya R
RegisterNumber: 212223230169
```

## SOURCE CODE:

```
import java.util.*;

class Person
{
    String name;
    int age;
}
class Student extends Person
{
    int marks;
    public String calculateGrade() 
    {
        if (marks >= 90) return "A";
        else if (marks >= 75) return "B";
        else if (marks >= 50) return "C";
        else return "F";
    }
    
    public void display()
    {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Marks: " + marks);
        System.out.println("Grade: " + calculateGrade());
    }
}

public class Main 
{
    public static void main(String[] args) 
    {
        Scanner sc = new Scanner(System.in);
        Student s = new Student();
        s.name = sc.nextLine();
        s.age = sc.nextInt();
        s.marks = sc.nextInt();
        s.display();

        sc.close();
    }
}
```


## OUTPUT:

<img width="511" height="626" alt="image" src="https://github.com/user-attachments/assets/26874b61-2846-404a-846b-7c8abe753078" />


## RESULT:
Thus, the program to create a Super class with fields using inheritance is written and executed successfully.

