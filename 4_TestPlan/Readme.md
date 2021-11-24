
# TEST PLAN:

[!image](https://i0.wp.com/onecore.net/wp-content/uploads/2014/11/Basic-Calculator.png?w=314&ssl=1)

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


