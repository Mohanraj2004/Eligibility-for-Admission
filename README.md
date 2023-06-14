#EX-NO-1 Eligibility-for-Admission

## Aim:
To write C# program to find the eligibility for admission to an engineering course.

## Algorithnm:
### Step 1:
Create a new Class named admission.

### Step 2:
Create variable of respective data types to store marks & name.
### Step 3:
Calculate the total and store it.
### Step 4:
The Conditions for admission are:

     * Marks in maths >= 65 & Marks in physics >=55 & Marks in chemistry >=50
     * Total marks in all three subjects >= 180 or total in maths and physics >= 140
### Step 5:
Using Nested if check whether the person is eligible or not for admission based on above conditions.
### Step 6:
Print the status for admission.
### Step 7:
End of the Program.
## Program:
```
Developed by: Mohan Raj
Reg No: 212221230065
```
```c#
using System;
namespace Students
{
    class program
    {
        static void Main(string[] args)
        {
            string name;
            Console.WriteLine("Enter the student name:");
            name = Console.ReadLine();
            int m, p, c, tot1, tot2;
            Console.Write("Enter math mark:");
            m = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter physics mark:");
            p = Convert.ToInt32(Console.ReadLine());
            Console.Write("Enter chemistry mark:");
            c = Convert.ToInt32(Console.ReadLine());
            tot1 = m + p + c;
            tot2 = m + p;

            if (m >= 65 && p >= 55 && c >= 50)
            {
                if (tot1 >= 108 || tot2 >= 140)
                {
                    Console.WriteLine(name + " is eligible for engineering admission");
                }
                else
                {
                    Console.WriteLine(name + " is NOT eligible for engineering admission");
                }
            }
            else
            {
                Console.WriteLine(name + "is NOT eligible for engineering admission");
            }

        }
    }


}



```


## Output:
![r1](https://user-images.githubusercontent.com/94525786/225648681-7feea749-2e5a-437e-8ff7-9534eeb24137.png)
)


## Result:
Thus, a C# program to check the eligibility of a student on engineering admission has been executed successfully.
