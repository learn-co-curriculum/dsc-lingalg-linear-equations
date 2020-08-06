
# Systems of Linear Equations 

## Introduction

Linear algebra is a sub-field of mathematics concerned with vectors, matrices, and linear transforms between them. 
The first step towards developing a good understanding of linear algebra is to get a good sense of *what linear mappings and linear equations* are, *how these relate to vectors and matrices* and *what this has to do with data analysis*. Let's try to develop a basic intuition around these ideas by first understanding what linear equations are. 

## Objectives

You will be able to: 

- Describe a system of linear equations for solving analytical problems 
- Describe how matrices and vectors can be used to solve linear equations 
- Solve a system of equations using elimination and substitution 

## What are linear equations?

In mathematics, a system of linear equations (or linear system) is a collection of two or more linear equations involving the same set of variables. For example, look at the following equations: 

 <img src="https://render.githubusercontent.com/render/math?math=
3x %2b 2y - z = 0 \\
2x- 2y %2b 4z = -2 \\
-x %2b 0.5y - z = 0
"> 

This is a system of three equations in the three variables  <img src="https://render.githubusercontent.com/render/math?math=x"> ,  <img src="https://render.githubusercontent.com/render/math?math=y"> , and  <img src="https://render.githubusercontent.com/render/math?math=z"> . A solution to a linear system is an assignment of values to the variables in a way that *all the equations are simultaneously satisfied*. A solution to the system above is given by:

 <img src="https://render.githubusercontent.com/render/math?math=
x = 1 \\
y = -8/3 \\
z = -7/3
"> 

These values make all three equations valid. The word "system" indicates that the equations are to be considered collectively, rather than individually.

## Solving linear equations

A system of linear equations can always be expressed in a matrix form. Algebraically, both of these express the same thing. Let's work with an example to see how this works: 

### Example 

Let's say you go to a market and buy 2 apples and 1 banana. For this, you end up paying 35 pence. If you denote apples by  <img src="https://render.githubusercontent.com/render/math?math=a"> and bananas by  <img src="https://render.githubusercontent.com/render/math?math=b"> , the relationship between items bought and the price paid can be written down as an equation - let's call it Eq. A: 

 <img src="https://render.githubusercontent.com/render/math?math=2a %2b b = 35">  (Eq. A)

On your next trip to the market, you buy 3 apples and 4 bananas, and the cost is 65 pence. Just like above, this can be written as Eq. B:

 <img src="https://render.githubusercontent.com/render/math?math=3a %2b 4b = 65"> (Eq. B)

These two equations (known as a simultaneous equations) form a system that can be solved by hand for values of  <img src="https://render.githubusercontent.com/render/math?math=a"> and  <img src="https://render.githubusercontent.com/render/math?math=b"> i.e., price of a single apple and banana.
 

Let's solve this system for individual prices using a series of eliminations and substitutions:

**Step 1:** Multiply Eq. A by 4

 <img src="https://render.githubusercontent.com/render/math?math=8a %2b 4b = 140"> (Eq. C)

**Step 2 :** Subtract Eq. B from Eq. C

 <img src="https://render.githubusercontent.com/render/math?math=5a = 75"> which leads to  <img src="https://render.githubusercontent.com/render/math?math=a = 15"> 

**Step 3:** Substitute the value of  <img src="https://render.githubusercontent.com/render/math?math=a"> in Eq. A

 <img src="https://render.githubusercontent.com/render/math?math=30 %2b b = 35"> which leads to  <img src="https://render.githubusercontent.com/render/math?math=b = 5"> 

So the price of an apple is 15 pence and the price of the banana is 5 pence. 

## From equations to vectors and matrices

Now, as your number of shopping trips increase along with the number of items you buy at each trip, the system of equations will become more complex and solving a system for individual price may become very expensive in terms of time and effort. In these cases, you can use a computer to find the solution.

The above example is a classic linear algebra problem. The numbers 2 and 1 from Eq. A and 3 and 4 from Eq. B are linear coefficients that relate input variables a and b to the known output 15 and 5.

Using linear algebra, we can write this system of equations as shown below: 

<img src="images/ss.png" width = "320">

You see that in order for a computational algorithm to solve this (and other similar) problems, we need to first convert the data we have into a set of matrix and vector objects. Machine learning involves building up these objects from the given data, understanding their relationships and how to process them for a particular problem. 

Solving these equations requires knowledge of defining these vectors and matrices in a computational environment and of operations that can be performed on these entities to solve for unknown variables as we saw above. We'll look into how to do this in upcoming lessons. 

## Summary

In this lesson, you learned how a system of linear (simultaneous) equations can be solved using elimination and substitution, and also, how to covert these problems into matrices and vectors to be processed by computational algorithms. In the next couple of lessons, we'll look at how to describe these entities in Python and NumPy and also how to perform arithmetic operations to solve these types of equations.
