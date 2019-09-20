---
layout: post
title: Calculator v.1.0
categories: C# Programming
---
To display something in the C# console the command is:

```csharp
Console.WriteLine("Hello World");
```

This needs to be within the: 
```csharp
static void Main(){      }
```

```csharp
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Console_App
{
    class Program
    {
        static void Main(string[] args)
        {
            //Programming Intro
            Console.WriteLine("-Calculator 1.0-");
            calculation();
        }
        public static void calculation()
        {
            //Declaring variables
            string tempAsdm;
            int asdm;
            string tempNum;
            double a;
            double b;
            double c;

            //Picking calculation methods
            Console.WriteLine("Input 1 for addition, 2 for subtraction, 3 for division, or 4 for multiplication.");
            tempAsdm = Console.ReadLine();
            asdm = Convert.ToInt32(tempAsdm);

            //Calculations
            if (asdm == 1)
            {
                Console.WriteLine("Input value A;");
                tempNum = Console.ReadLine();
                a = Convert.ToDouble(tempNum);
                Console.WriteLine("Input value B;");
                tempNum = Console.ReadLine();
                b = Convert.ToDouble(tempNum);
                c = a + b;
                Console.WriteLine(a + " + " + b + " = " + c);
            }
            else if (asdm == 2)
            {
                Console.WriteLine("Input value A;");
                tempNum = Console.ReadLine();
                a = Convert.ToDouble(tempNum);
                Console.WriteLine("Input value B;");
                tempNum = Console.ReadLine();
                b = Convert.ToDouble(tempNum);
                c = a - b;
                Console.WriteLine(a + " - " + b + " = " + c);
            }
            else if (asdm == 3)
            {
                Console.WriteLine("Input value A;");
                tempNum = Console.ReadLine();
                a = Convert.ToDouble(tempNum);
                Console.WriteLine("Input value B;");
                tempNum = Console.ReadLine();
                b = Convert.ToDouble(tempNum);
                c = a / b;
                Console.WriteLine(a + " / " + b + " = " + c);
            }
            else if (asdm == 4)
            {
                Console.WriteLine("Input value A;");
                tempNum = Console.ReadLine();
                a = Convert.ToDouble(tempNum);
                Console.WriteLine("Input value B;");
                tempNum = Console.ReadLine();
                b = Convert.ToDouble(tempNum);
                c = a * b;
                Console.WriteLine(a + " * " + b + " = " + c);
            }
            else
            {
                Console.WriteLine("Inputted value invalid, try again.");
            }
            Console.ReadLine();
            calculation();
        }
    }
}
```
