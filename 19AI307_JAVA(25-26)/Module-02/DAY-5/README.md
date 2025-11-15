# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Create a class Student with variables name, rollNumber. Create a method setDetails(String name, int rollNumber),and display them.

## AIM:
To create a class Student with variables name, rollNumber. Create a method setDetails(String name, int rollNumber),and display them.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class Student with variables name and rollNumber.
4.	Create a method setDetails(String name, int rollNumber) to assign values to the variables.
5.	Create another method display() to print the student details.
6.	In main(), create an object of Student.
7.	Call setDetails() to set the student’s name and roll number.
8.	Call display() to show the details.
9.	End the program.

## PROGRAM:
 ```
/*
Program to implement a Access Modifiers using Java
Developed by: RAMYA R
RegisterNumber:  212223230169
*/
```

## SOURCE CODE:
```
import java.util.Scanner;

class Student {
    String name;
    int rollNumber;
    
    public String getName()
    {
        return name;
    }
    public void setName(String name)
    {
        this.name = name;
    }
    
    public int getroll()
    {
        return rollNumber;
    }
    public void setroll(int rollNumber)
    {
        this.rollNumber = rollNumber;
    }
    
    void display()
    {
        System.out.println("Name: "+name);
        System.out.println("Roll Number: "+rollNumber);
    }
}

class prog 
{
    public static void main(String[] argv)
    {
        Scanner sc = new Scanner(System.in);
        Student obj = new Student();
        
        obj.setName(sc.nextLine());
        obj.setroll(sc.nextInt());
        
        obj.display();
    }
}
```


## OUTPUT:

<img width="685" height="410" alt="image" src="https://github.com/user-attachments/assets/6be1b369-d213-4241-aca1-028749a780fa" />


## RESULT:
Thus, the program sets the student’s name and roll number using the setDetails method and displays them using the display method.
