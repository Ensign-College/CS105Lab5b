Lab 4a
======

Submit your finished code to the Dropbox. You will need to pass off the lab with the TA or tutor during their office hours (their information is in the CS 105 Course Information section of the Class Resources 
module), or the instructor in class. Follow the CS 105 Formatting Guide which is also found in the CS 105 Course Information section.

Read the instructions carefully. Make sure your output matches the example run.

Objectives:
===========

In this lab, you will learn how to do the following:

-   Use a while loop or a do-while loop
-   Understand the issues behind users entering in the wrong type of data
-   Use a try/catch statement
-   Perform Input validation on User Input

Structure:
==========

Create the following structure in Eclipse for this lab.

-   **Package Name: w**eek4
-   **Class Name: **Lab4aPonder
-   **Class Name: **Lab4a

Investigate and Ponder:
=======================

Failure to run this experiment and discuss the results with your partner before you attempt to pass off Lab4a will result in a failed pass off.

**Step 1:** Create a class named Lab4aPonder

**Step 2: ** Enter the following code into the Lab4aPonder class:

*public static void main(String[] args) {*

*// Use Scanner for getting Input from user*\
*Scanner in = new Scanner(System.in);                           //Input Scanner*

*System.out.print("Please enter a number: ");*\
*String input = in.nextLine();*

int num1 = Integer.parseInt(input);

*System.out.printf("You entered the number " + num1);*

*}//end of method main()*

**Step 3:** Run the program and enter a number at the prompt.  The program should run without errors.

**Step 4:** Now run the program again and enter the word **"pizza"** at the prompt.  What happens?

**Step 5:** Discuss with your partner why you got an error running the same code with different input. 

Input Validation:
=================

As Java programmers, we can write code to allow users to input strings, integers, doubles, etc.  However, we can't guarantee the user will enter the type of data we are requesting.  Input Validation is the 
technique of ensuring the user enters the correct type of data before data processing begins.  One way to do this is to use while loops.

In a flow diagram, input validation might look something like this:

![Input Validation Flow.jpg](https://ensign.instructure.com/courses/16292/files/5757289/preview)

In pseudo code, input validation might look something like this:

*Initialize control variable as invalid*

*do {*

*Ask the user to enter some data.*

*If the data is valid, set control variable as valid.*

*Otherwise, print an error message and stay in the loop.*

*} while (the control variable is invalid)*

Program: Input validation
=========================

Write a program that asks the user to enter a whole number. Use input validation to ensure the user entered a valid whole number. Perform simple math on the number to ensure your input validation routine 
worked as expected. Display the results.

**Step 1:** Create a class, Lab4a with a main() method

**Step 2:** Declare a Scanner object, i**n.**

**Step 3: **Declare a String variable, input,  and initialize it to "".

**Step 4:** Declare three integer variables **num1, num2 and num3** and initialize them to 0.

**Step 5:** Declare a boolean control variable, **valid**, and set it to false.

**Step 6:** Create a do-while loop using the** valid** control variable.

*do {*\
*} while (!valid);*

**Step 7:** Ponder and discuss with your partner:

-   Why is it important to test **!valid** instead of **valid**?
-   Why did you set **valid** to **false** in Step 5?

**Step 8:** In the body of the do-while loop, prompt the user to enter a number.

**Step 9:** Use in.nextLine() to get the input from the user.

**Step 10:** Create a try/catch statement inside your while loop.  Use the standard Exception to catch all exceptions in the catch statement.

The program should now look something like this:

 *    //Declare variables*

*     do{*

*          System.out.print("Please enter a number: ");*

*          input = in.nextLine();*

*          try{*

*          } catch (Exception e) {*

*          } //end of try/catch*

*     }while (!valid};*

**Step 11:** In the try block, convert the user's input into an integer and store it in num1 using Integer.parseInt()

**Step 12:** If the parseInt() statement ran without issue, then you can set valid = true so that the program will exit the do-while loop once a valid integer has been entered.  Add the following statement to 
the try block:

*valid = true;*

**Step 13:** If the user entered something other than a valid integer, the code in the catch block will run without crashing the program.  Display a helpful message prompting the user to correct the error 
inside the catch block:

*System.out.println("Error: Please enter a whole number.\n");*

**Step 14:** Outside of the do-while loop, perform the following mathematical calculations:

-   Set num2 to equal num1 + 1000.
-   Set num3 to equal num1 * 2.

**Step 15:** Print out **num1, num2 and num3** as shown in the example run.

**Step16:** Discuss with your partner why you used a **do-while** loop rather than a w**hile** loop.

Key Program Requirements:
=========================

-   Follow each of the steps above and discuss the results with your partner as described.
-   Submit the following .java file:
-   -   Lab4a.java

Example Run:
============

*Please enter a number: Pizza*\
*Error: Please enter a whole number.*

*Please enter a number: Uno*\
*Error: Please enter a whole number.*

*Please enter a number: 42*\
*num1 = 42.*\
*num2 = 1042.*\
*num3 = 84.*Lab 5b
======

Submit your finished code to the Dropbox. You will need to pass off the lab with the TA or tutor during their office hours (their information is in the CS 105 Course Information section of the Class Resources 
module), or the instructor in class. Follow the CS 105 Formatting Guide which is also found in the CS 105 Course Information section.

Read the instructions carefully. Make sure your output matches the example run.

Objectives:
===========

In this lab, you will learn how to do the following:

-   Modify an old program to make it more flexible and efficient
-   Modify a series of similar and repetitive calculations to use a FOR loop instead
-   Perform input validation on user input of type double

Structure:
==========

Create the following structure in Eclipse for this lab.

**Package Name:** week5\
**Class Name:** Lab5b

Program: Improved Interest Calculator
=====================================

In Lab 2d, you were asked to create a program that would calculate the balance of a savings account after 6 months. In this Lab, we will revisit the monthly interest calculation program but add one additional 
feature. In this program you will add the ability for the user to enter the number of months they plan on saving.

Write a program that asks the user:

-   the amount to be deposited each month (double)
-   the annual interest rate percentage (double)
-   the number of months they wish to save (int)

Your program must perform input validation on all three numbers entered by the user to ensure the deposited amount and annual interest are doubles and that the number of months is an integer.

Print out the monthly balance over the specified savings duration. Remember to include both the first and last month of your period. 

After the program has finished, ask the user if they would like to try another calculation. Use input validation to ensure the user answers with a 'Y' or 'N'. Keep the program running in an infinite loop 
until the user indicates they want to quit.

Key program requirements:
=========================

-   Your program must perform input validation on all three numbers entered by the user to ensure they are appropriately doubles or ints.
-   Your program must perform input validation on the "Try another calculation (Y/N): " question to ensure the answer entered by the user is either a 'Y' or 'N'.
-   Make sure that your program follows the Example Run shown below and that the balance shown each month is rounded to two digits, includes commas,  and includes a '$'.
-   Submit the following .java file:
    -   Lab4d.java

Hint:  To add commas to your formatted string, simply add a comma to your format scheme.

#### *Example:  printf("Balance is: $%**,**.2f",balance)*

Example Run:
============

*This program will ask the user for a monthly deposit, an annual interest rate and the number of months the user plans on saving.*\
*It will then show the monthly balance over the period of planned savings.*

*Please enter the amount to be deposited each month: a lot!*\
*Invalid response: Please enter a whole number.*

*Please enter the amount to be deposited each month: 250.50*\
*Please enter the annual interest rate: 3.75*\
*Please enter the number of months you plan to save: 18*

*The following table shows the balance of the account for each month of the designated savings period.*\
*Month              Balance*\
*Month 1:         $251.28*\
*Month 2:         $503.35*\
*Month 3:         $756.21*\
*Month 4:         $1,009.85*\
*Month 5:         $1,264.29*\
*Month 6:         $1,519.52*\
*Month 7:         $1,775.56*\
*Month 8:         $2,032.39*\
*Month 9:         $2,290.02*\
*Month 10:      $2,548.46*\
*Month 11:      $2,807.71*\
*Month 12:      $3,067.76*\
*Month 13:      $3,328.63*\
*Month 14:     $3,590.32*\
*Month 15:     $3,852.82*\
*Month 16:     $4,116.14*\
*Month 17:     $4,380.29*\
*Month 18:     $4,645.26*\
*Would you like to make another calculation? (Y/N): n*
