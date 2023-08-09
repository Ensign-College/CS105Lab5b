Lab 5b
======

Submit your finished code to the Dropbox. You will need to pass off the lab with the TA or tutor during their office hours (their information is in the CS 105 Course Information section of the Class Resources module), or the instructor in class. Follow the CS 105 Formatting Guide which is also found in the CS 105 Course Information section.

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

In Lab 2d, you were asked to create a program that would calculate the balance of a savings account after 6 months. In this Lab, we will revisit the monthly interest calculation program but add one additional feature. In this program you will add the ability for the user to enter the number of months they plan on saving.

Write a program that asks the user:

-   the amount to be deposited each month (double)
-   the annual interest rate percentage (double)
-   the number of months they wish to save (int)

Your program must perform input validation on all three numbers entered by the user to ensure the deposited amount and annual interest are doubles and that the number of months is an integer.

Print out the monthly balance over the specified savings duration. Remember to include both the first and last month of your period. 

After the program has finished, ask the user if they would like to try another calculation. Use input validation to ensure the user answers with a 'Y' or 'N'. Keep the program running in an infinite loop until the user indicates they want to quit.

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
