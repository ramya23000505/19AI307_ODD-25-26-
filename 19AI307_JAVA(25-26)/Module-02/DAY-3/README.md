# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## AIM:
To write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create a class BankAccount with private variables accountNumber and balance.
4.	Provide public setter methods to assign values to accountNumber and balance.
5.	Provide public getter methods to return the values of accountNumber and balance.
6.	In the main() method, create an object of BankAccount.
7.	Use the setter methods to store account number and balance.
8.	Use the getter methods to display the stored values.
9.	End the program.


## PROGRAM:
 ```
/*
Program to implement a Access Specifiers using Java
Developed by: RAMYA R
RegisterNumber:  212223230169
*/
```

## SOURCE CODE:

```
import java.util.Scanner;

class BankAccount 
{
    
    private String accountNumber;
    private double balance;

    
    public String getAccountNumber() 
    {
        return accountNumber;
    }
    public void setAccountNumber(String accountNumber) 
    {
        this.accountNumber = accountNumber;
    }
    
    public double getBalance() 
    {
        return balance;
    }
    public void setBalance(double balance) 
    {
        this.balance = balance;
    }
    
    void display()
    {
        System.out.println("Account Number: "+accountNumber);
        System.out.println("Balance: "+balance);
    }
}
public class Main
{
    public static void main(String[] argv)
    {
        Scanner sc = new Scanner(System.in);
        BankAccount obj = new BankAccount(); 
        
        obj.setAccountNumber(sc.next());
        sc.nextLine();
        obj.setBalance(sc.nextDouble());
        
        obj.display();
    }
}
```
## OUTPUT:
<img width="841" height="473" alt="image" src="https://github.com/user-attachments/assets/89a63b24-05d6-4084-b8f0-cec5ff2cb45b" />


## RESULT:
Thus, the program successfully stores the account number and balance using setter methods and retrieves them using getter methods to display the account details.
