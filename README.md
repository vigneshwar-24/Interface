# Interface

## Aim:
To Develop a small bank application by declaring deposit() and withdrawal() as abstract methods in the interface. Get the choice from the user whether to perform withdrawal or deposit operation. After the operation completes, display the balance amount.

## Algorithm:
### Step 1:
Create an Interface.
### Step 2:
Create a child class.
### Step 3:
Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.
### Step 4:
Create those 2 functions in the child class and perform respective operation.
### Step 4:
Use while loop and and switch case to Get the choice from the user whether to perform withdrawal or deposit operation.
### Step 5:
After performing the functions display the remaining balance of the user.

## Program:
```
Developed by  : S.Sham Rathan
Resgister no. : 212221230093

using System;
namespace ConsoleApp21
{
    class Program
    {
        public interface bank
        {
            void deposit(int amount);
            void withdrwal(int amount);
        }
        public class bankEx
        {
            int balance = 5000;  
                public void deposit(int amount)
            {
                balance += amount;
                Console.WriteLine(balance);
            }
            public void withdrwal(int amount)
            {
                balance -= amount;
                Console.WriteLine(balance);

            }
            public static void Main()
            {
                bankEx obj = new bankEx();
                Console.WriteLine("1.Deposit\n2.Withdrawl");
                int ch = Convert.ToInt32(Console.ReadLine());
                if(ch==1)
                {
                    Console.WriteLine("Enter the amount to be deposited:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Balance");
                    obj.deposit(amount);
                }
                else if(ch==2)
                {
                    Console.WriteLine("Enter the amount to be withdrawed:");
                    int amount = Convert.ToInt32(Console.ReadLine());
                    Console.WriteLine("Balance");
                    obj.withdrwal(amount);

                }
            }
        }

    }
}

```


## Output:

![20](https://user-images.githubusercontent.com/93587823/203898394-e7a72e7e-a299-4a99-89c7-d60ab8ee0708.png)

## Result:
C# program to develop a bank application using interface is implemented successfully.
