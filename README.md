# Pattern

## Aim:
To write a C# program for a pascal's triangle.

## Equipment Required:
Visual Studio

## Algorithm:
Step 1:
Create a class.

Step 2:
Use nested for loop.

Step 3:
End the for loop.

## Program:

Developed By: S.THIRISHA
Reg no: 212222230160
```
using System;
namespace condition
{
    public class pascal
    {
        public static void Main(string[] args)
        {
            int rows , Val = 1;
            Console.Write("Enter number of rows: ");
            rows = Convert.ToInt32(Console.ReadLine()); 
            for (int i = 0; i < rows; i++)
            {
                for (int blank = 1; blank < rows - i; blank++)
                {
                    Console.Write(" ");
                }
                for (int j = 0; j <= i; j++)
                {
                    if (i == 0 || j == 0)
                    {
                        Val = 1;
                    }
                    else
                    {
                        Val = Val * (i - j + 1) / j;
                    }
                    Console.Write(Val + " ");
                }
                Console.WriteLine();
            }
        }
    }
}
```

## Output:
![267204380-9ad13be6-fd2f-4b88-a84e-0fa4d4feca81](https://github.com/Thirisha-s/C-Pattern/assets/120380280/dfaa6bbd-ac02-47d7-bf43-c6701010eb77)

![267204423-ce39f3b6-5f66-43e6-aef4-e8ba9ee5e274](https://github.com/Thirisha-s/C-Pattern/assets/120380280/cd62bdf2-59ea-4fa3-8505-644bda3022db)


## Result:
Thus the C# program to print the pascal's triangle is executed successfully.
