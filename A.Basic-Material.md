# 🐇 Competitive Programming Notes (C++)

Hello, this is basically my notes for the basics to get ready for **competitive programming**,  
or if you need to do a **coding interview** for your new job!

For this document I will be using **C++** because I have been using C for quite a while.

We will talk about several things today with some examples of code questions of *"competitive coding"*.

---

## 📌 Homepage / Navigation

- [A. Basic Syntax C++](#a-basic-syntax-c)
- [B. Variables and Data Type](#b-variables-and-data-type)
- [C. Operator](#c-operator)
- [D. If / Else](#d-if--else)
- [E. Repetition](#e-repetition)
- [F. Scope](#f-scope)
- [G. Function / Recursion](#g-function--recursion)
- [H. Library C++](#h-library-c)
- [I. Example Code Questions](#i-example-code-questions)
- [Complexity Time](#complexity-time)
- [Tips and Tricks](#tips-and-tricks)

---

## A. Basic Syntax C++

1. `cin` -> which is basically used to input your variable  
2. `cout` -> which is basically used to output your data  

You'd usually write something like:
```cpp
int x;
cin >> x;
cout << x;
```

Please do note that you need to use '>>' when using cin
and you need to use '<<' to use cout , dont get them mixed up!

## B. Variables and Data Type
Within the coding environment, sometimes you need to declare a variable, like a math question.

There are many types of variables and data types in C++.

For example, boba has 5 watermelons, and in the coding environment you can also declare something like this:
```cpp
int watermelon = 5;
# note that every line of code in C++ will need to end with ;
```
Or if you need decimals, then I usually use float or double:
```cpp
float watermelon = 5.0;
double watermelon = 5.0;
```
There are some rare cases where you'd usually like to use long long,
but this is very rare in competitive programming so we can just go ahead and skip that part.

Now how do we declare a word — or even a sentence?
If someone would like to say that they have watermelon and they use the word W for a codename:
```cpp
char codename = 'W';
string fruit = "watermelon";
```

I usually add one more variable which is a bool,
basically it is just a flag to make you know whether the data is true or false.

## C. Operator
Operators are just basically math equation that you usually see everywhere, like when you want tpo add something, division, minus, modulos, etc.
```cpp
int x = 6;
cout << 6%3;
```

## D. If / Else
If - Else is a very common practice in the competitive coding, you usually use it if you have a condition that your program must fulfill.
Now for example how should we know if a number is even? this is a very common question in coding, and we can solve this with an if - else statement
```cpp
int x = 6;
if (x % 2 == 0 ) {
  cout << "This is an even number";
}
else {
  cout << "This is an odd number";
}
```
Explanation : Now in the code above the program will try to do some math operation 'modulo' to know whether we can divide 6 with the number 2 or not. If it returns zero (which means that yes 6 can be divided by 2) , if it doesnt return zero (else) that means the number is no divisible by two, thus making it an odd number.

## E. Repetition
Repetition is also one of the most common questions that we have in a coding competition. Usually we use two things for repetition , maybe if you already hear nested loops and while statemnets, then you should be able to do it easily. Repetitions are basically when you want to do something until your statement is fulfilled.

1. For loops
For ( 

3. While Statements


4. Recursion 


## F. Scope

## G. Function 
Function is something similar like a math formula 

## H. Library C++

## I. Example Code Questions
1. Example Problem 1
Problem : 
Given integer N
Determine if N is a prime number or not

Constraint : 1 <= N <= 10^9
Time Limit : 1 Second

Answer : 
```cpp

```

Explanation : 

2. Example Problem 2
Problem : 
You are given two positive integers , N and M 
Please calculate N^M mod 10^9

Constraint : 1 <= N, M <= 10^9
Time Limit : 1 Second

Answer : 
```cpp

```

Explanation :   
3. Example Problem 3
Problem : 
You are given an array A of N positive integers 
Find the largest contigous subarray with its sum <= K

Constraint : 1 <= N, M <= 10^5, 1 <= A[i] <= 10^9, 1 <= K <= 10^14

Answer : 
```cpp

```
Explanation :   

## Complexity Time

## Tips and Tricks


