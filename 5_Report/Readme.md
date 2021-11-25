# Requirements

The Calculator should contain 0-9 numbers.

The Calculator must contain Addition,Subtraction,Multiplication Division,Square and Squareroot

## Introduction
 
A basic calculator is sometimes referred to as a 4-function calculator

A calculator is a machine which allows people to do math operations more easily. For example, most calculators will add, subtract, multiply,Square and Squareroot.

## Research
 We had Researched on how to build and how the calculator can be customer oriented.

## Cost and Features and Timeline

The cost of the calculator should be low as well as it should contain all the basic features.

## SWOT_ANALYSIS

Calculator are long-lasting, and they have almost all kinds of calculators such as basic, scientific, graphing, financial etc.

## STRENGTHS 
The ultimate strength of Calculators is its innovative and user-friendly products. calculators are long-lasting, and they have almost all kinds of calculators such as basic, scientific, graphing, financial, etc. Their technological expertise is one of the greatest. Workforce with more than 10000 people and powerful marketing has made it a market giant among tech-based businesses. Casio has the trust of people, which is valuable than any other strength. Also, they have a huge loyal customer base all over the world.
## WEAKNESSES
Casio has a strong brand image for manufacturing calculators, but at the same time, this brand image works as a stereotype for them. It is Casio’s weakness. Casio has many other wonderful product lines other than calculators, but people don’t rely on them much when buying something than calculators. Even though this company has a wide range of product portfolio, it’s prolonged when it comes to launching new products matching the changing customer’s needs. As a result, those who want a change in their electronics accessories tend to avoid Casio.
## OPPORTUNITIES
The tech-based market has a huge opportunities in capturing the youth market. And Casio is comparatively already one step ahead than other companies. Because since the beginning of childhood, we got introduced to Casio as a helping partner in mathematics. We accepted it as a companion, and an emotional attachment grew. So if Casio launches any innovative products for the youth generation, they won’t think much before give it a try. Also, sponsoring different events and working towards the educational improvement campaigns can add more segments to their customer base.
## THREATS 
Although Casio enjoys a substantial competitive advantage in the calculator business, strong competitors such as Nikon, Fastrack, Panasonic, Sony, Pentax, etc. are emerging daily and gaining popularity among people. Also, due to the stereotype image for “Only a calculator brand,” it’s getting hard for Casio to enter sports and other tech-product lines as there’re already many strong brands are ruling. Their slower growth in technological innovation will also bring a significant threat in the upcoming dynamic world.

# 4w's and 1H

## Who
   
The First solid state electronic was created by Blaise pascal.

## What

An electronic Calculator is typically a portable electronic device used to perform.

## When

The First calculator was build in early 1960s. and then later updated to pocket calculator in 1970s

## Where

Calculator was developed by intel for the japanese calculator company busicom

## How

Calculation is being able to perform all four airthmatic operations with minimal human interaction.

# Detail requirements
## High Level Requirements

This project can be implemented by using c language in both windows and linux os.

This project will require all the input from user end and then it can perform required tasks on it

It should contain **Addition,Subtraction,Multiplication,Square and Squareroot**

# Design

## FlowChart

![image](https://user-images.githubusercontent.com/80145154/142749386-eda9c48e-7d69-4668-bff1-e8b425f71ddb.png)

## Beheavioural Diagram

![image](https://imgur.com/KtW56.jpg)

# Implimentation

## Source code

#include <stdio.h>  
#include <conio.h>  
#include <math.h>  
#include <stdlib.h>  
      
  
int addition();  
int subtract();  
int multiply();  
int divide();  
int sq();  
int sqrt1();  
void exit();  
  
int main()  
{  
      
    int op;  
    do  
    {  
          
        printf (" Select an operation to perform the calculation in C Calculator: ");  
        printf (" \n 1 Addition  \t \t 2 Subtraction \n 3 Multiplication \t 4 Division \n 5 Square \t \t 6 Square Root \n 7 Exit \n \n Please, Make a choice ");      
          
        scanf ("%d", &op);   
      
      
     
    switch (op)  
    {  
        case 1:  
            addition();  
            break; 
              
        case 2:  
            subtract();  
            break;  
              
        case 3:  
            multiply(); 
            break;   
              
        case 4:  
            divide();
            break;  
              
        case 5:  
            sq(); 
            break; 
              
        case 6:  
            sqrt1();  
            break; 
              
        case 7:  
            exit(0);   
            break;   
              
        default:  
            printf(" Something is wrong!! ");  
            break;                        
    }  
    printf (" \n \n ********************************************** \n ");  
    } while (op != 7);  
      
  
    return 0;        
}  
  
  
  

int addition()  
{  
    int i, sum = 0, num, f_num; 
    printf (" How many numbers you want to add: ");  
    scanf ("%d", &num);  
    printf (" Enter the numbers: \n ");  
    for (i = 1; i <= num; i++)  
    {  
        scanf(" %d", &f_num);  
        sum = sum + f_num;  
    }  
    printf (" Total Sum of the numbers = %d", sum);  
    return 0;  
}  
  

int subtract()  
{  
    int n1, n2, res;  
    printf (" The first number is: ");  
    scanf ("  %d", &n1);  
    printf (" The second number is: ");  
    scanf ("  %d", &n2);  
    res = n1 - n2;    
    printf (" The subtraction of %d - %d is: %d", n1, n2, res);  
}  
  
 
int multiply()  
{  
    int n1, n2, res;  
    printf (" The first number is: ");  
    scanf ("  %d", &n1);  
    printf (" The second number is: ");  
    scanf ("  %d", &n2);  
    res = n1 * n2;    
    printf (" The multiply of %d * %d is: %d", n1, n2, res);  
}  
  

int divide()  
{  
    int n1, n2, res;  
    printf (" The first number is: ");  
    scanf ("  %d", &n1);  
    printf (" The second number is: ");  
    scanf ("  %d", &n2);  
      
    if (n2 == 0)  
    {  
        printf (" \n Divisor cannot be zero. Please enter another value ");  
        scanf ("%d", &n2);        
    }  
    res = n1 / n2;    
    printf (" \n The division of %d / %d is: %d", n1, n2, res);  
}  
  
 
int sq()  
{  
    int n1, res;  
    printf (" Enter a number to get the Square: ");  
    scanf ("  %d", &n1);  
      
    res = n1 * n1;    
    printf (" \n The Square of %d is: %d", n1, res);  
}  
  
  
int sqrt1()  
{  
    float res;  
    int n1;  
    printf (" Enter a number to get the Square Root: ");  
    scanf ("  %d", &n1);  
  
    res = sqrt(n1);   
    printf (" \n The Square Root of %d is: %f", n1, res);  
}  



# TEST PLAN:

![image](https://i0.wp.com/onecore.net/wp-content/uploads/2014/11/Basic-Calculator.png?w=314&ssl=1)

## Table no: High level test plan

| **Test ID** | **Description**                                              | **Exp I/P** | **Exp O/P** | **Actual Out** |**Type Of Test**  |    
|-------------|--------------------------------------------------------------|------------ |-------------|----------------|------------------|
|  H_01       |Square of two numbers                                         |Square of 4   |16            |16               |Square based      |
|  H_02       |Square root of the number                                     |Square root of 5|2.23        |2.23             |Square root based    |


## Table no: Low level test plan

| **Test ID** | **Description**                                              | **Exp IN** | **Exp OUT** | **Actual Out** |**Type Of Test**  |    
|-------------|--------------------------------------------------------------|------------|-------------|----------------|------------------|
|  L_01       |Addition of two numbers                                       |  10+4      | 14          | 14             |Addition based    |
|  L_02       |Subtraction of two numbers                                    |  10-4      | 6           |  6             |Subtraction based    |
|  L_03       |Multiplication of two numbers                                 |  10*4      | 40          | 40             |Multiplication based    |
|  L_04       |Division of two numbers                                       |  10/2      | 5           |  5             |Division based      |

# HIGH LEVEL TEST PLAN

1.Check if the calculator is a normal calculator or a scientific calculator.

2.Verify that all the buttons are present and text written on them is readable.

3.Check the arithmetic operations are working fine- +, -, /, * etc.

4.Verify that BODMAS is applied in case of complex queries and the correct result is returned.

5.Verify that the calculator gives the correct result in case of operations containing decimal numbers.

# LOW LEVEL TEST PLAN

1.Verify the number of digits allowed to enter in the calculator for any operation.

2.Verify the limit of the response value.

3.Verify the functioning of memory functions.

4.Check if the calculator allows navigating through previous calculations

5.Verify that on pressing two operators one after the other, the latest one will override the previous operator.




Status:All the other Implementations will be done at later Part.


##  Low level Requirements

It should contain numerical values from 0-9

## Output images
![image](https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/Addition.png)
![image](https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/Subtraction.png)
![image](https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/Multiplication.png)
![image](https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/Division.png)
![image](https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/Square.png)
![image](https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/Square%20root.png)

## Video

https://github.com/DodlaSreekanth/M1_Application_Caluculator/blob/main/6_Images%20and%20Videos/video-for-caluculator-project_.mp4






                                                          

