# Check-Whether-or-Not-the-Year-is-a-Leap-Year-in-Java

Given an integer input for the year, the objective is to check whether or not the user given input “year” is a Leap year or not. In order to do so we check if the integer input satisfies the conditions for a leap year mentioned below. Therefore, we write a Java code to check and tell if it’s a leap year or not. Some of the methods to check for leap year are mentioned below

Method 1: Using if-else Statements 1
Method 2: Using if-else Statements 2
Method 3: Using Ternary Operator
Method 4: Bonus Boolean method
We’ll discuss the above-mentioned methods in detail in the upcoming sections. Before we get to coding check the blue box below for better understanding.

Conditions for Leap Year
For any year to be a leap year the following two conditions must be checked. If the year satisfies either of the conditions, it's considered a leap year. Following are the conditions
1. The year must be divisible by 400.
2. The year must be divisible by 4 but not 100.
Method 1: Using if-else Statements 1
Working
For the input integer “year” we perform the following

Check if the year variable is divisible by 400.
Check if the year variable is divisible by 4 but not by 100.
If the above conditions are satisfied, print it’s a Leap year. It’s not a Leap Year otherwise.
Let’s try and implement the above mentioned logic in Java Language.

Java Code
Run
// Leap year program in Java
// If the year satisfies either of the conditions, it's considered a leap year -
// 1. The year must be divisible by 400.
// 2. The year must be divisible by 4 but not 100.
public class Main{
   public static void main (String[]args)
   {

     int year = 2020;

     if (year % 400 == 0)
       System.out.println (year + " is a Leap Year");

     else if (year % 4 == 0 && year % 100 != 0)
       System.out.println (year + " is a Leap Year");

     else
         System.out.println (year + " is not a Leap Year");

   }
 }
Output
2020 is a Leap Year
While loop in C
Related Pages
Greatest of two numbers

Greatest of the Three numbers

Prime number

Prime number within a given range

Sum of digits of a number

Method 2: Using if-else Statements 2
Working
For a given integer variable “year”, we check for the following

If the year variable is divisible by 400 or is it divisible by 4 but not 100.
Print it’s a Leap Year if true, Print it’s not a Leap year otherwise.
Let’s implement the above logic in Java Language.

Java Code
Run
public class Main
 {
   public static void main (String[]args)
   {

     int year = 2020;

     if (year % 400 == 0 || (year % 4 == 0 && year % 100 != 0))
       System.out.println (year + " is a Leap Year");

     //not leap year
     else
         System.out.println (year + " is not a Leap Year");

   }
 }
Output
2020 is a Leap Year
Method 3: Using Ternary Operator
Working
In this method we’ll use the knowledge of ternary operators. To know more about ternary operators in C, check out Ternary operators in C.

For a given input integer variable “year”, we check for the following using the ternary operator

Check if the year variable is divisible by 400 or divisible by 4 but not 100.
If either of the above mentioned conditions are satisfied, print it’s a Leap Year. Print it’s not a Leap Year otherwise.
Let’s implement the above mentioned logic in Java Language.

Java Code
Run
public class Main
{
  public static void main (String[]args)
  {

    int year = 2019;
    
     int flag = (year%400 == 0) || (year%4==0 && year%100!=0 ) ? 1 : 0;
    if (flag ==1)
    {
        System.out.println (year + " is a Leap Year");
    }
    else
    {
         System.out.println (year + " is not a Leap Year");
    }
  }
}
Output
2019 is not a Leap Year
Method 4: Bonus Boolean Method
Java Code
Run
class Main {

    public static void main(String[] args) {

        // If the year satisfies either of the conditions, it's considered a leap year -
        // 1. The year must be divisible by 400.
        // 2. The year must be divisible by 4 but not 100.
        int year = 2020;
        boolean leap;

        if (year % 400 == 0)
            leap = true;

        else if (year % 4 == 0 && year % 100 != 0)
            leap = true;

        else
            leap = false;

        if (leap)
            System.out.println(year + " is a leap year.");
        else
            System.out.println(year + " is not a leap year.");
    }
}
Output
2020 is not a Leap Year
