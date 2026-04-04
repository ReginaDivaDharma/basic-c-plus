# 🐇 Competitive Programming Notes (C++)

Hello, this is basically my notes for the basics to get ready for **competitive programming**,  
or if you need to do a **coding interview** for your new job!

For this document I will be using **C++** because I have been using C for quite a while.
Please do remember that in coding you need to focus on translating algorithms instead of memorizing.

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
Usually you use String if you need to have some words. but please do note that string is actually a class. 

I usually add one more variable which is a bool,
basically it is just a flag to make you know whether the data is true or false.

An array is also a very , common practice with a coding practice , something similar like a matrix if you are familiar with it. 
And actually arrays have many different forms, there's a 2D array , 3D arrays , etc. But one thing that you need to know about arrays and their many nested things, it's quite simple, it's just an array inside of another array.
```cpp
int x [2][3] = {
  {0,1,2},
  {3,4,5)
}
```

## C. Operator
Operators are just basically math equation that you usually see everywhere, like when you want tpo add something, division, minus, modulos, etc.
```cpp
int x = 6;
cout << 6 % 3;
```

## D. If / Else
If - Else is a very common practice in the competitive coding, you usually use it if you have a condition that your program must fulfill.
Now for example how should we know if a number is even? this is a very common question in coding, and we can solve this with an if - else statement.
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
There are many uses for loops , it's basically saying , please do x while the value of x is still under the condition you have set. 

```cpp
for (int i = 0 ; i <=5 ; i++) {
  cout << i;
  i += 1;
}
``` 

2. While Statements
```cpp
int x = 10;
while ( x > 1 ) {
  cout << x ;
  x -= 1;
}
``` 

3. Recursion
Recursion is basically a function that calls upon itself again, and this is by far the most used thing in competitive programming. 
```cpp

``` 

## F. Scope


## G. Function 
Function is something similar like a math formula maybe if you are familiar with this f(x) = x + 5, this is basically a function ! the int main itself is also a function, you usually use it if you want to make your code easier to understand. So how do we use a function or make a new one? well see the codes down below!
```cpp
int f(x) {
  return x + 5;
}

int main () {
  int x;
  cin >> x;
  f(x);
}

``` 

## H. Library C++
C++ offers many new libraries that you can use in competitive programming, instead of making a sort by yourself , we already have a library for it now. We will dive in to this library more in data structure.

## I. Example Code Questions
1. Example Problem 1
Problem : 
Given integer N
Determine if N is a prime number or not

Constraint : 1 <= N <= 10^9
Time Limit : 1 Second

Answer : 
```cpp
#include <bits/stdc++.h>
using namespace std;

/*
The algorithm below is to solve how to know whether a number is a primary number ir not. 
But before we write the code let's understand what is a primary number itself first? 

Primary number is a number that can only be divided by one and itself. The numbers are usually odds and are a positive greater than one. Only number two is considered an even primary number.

Now let's think like a robot, how do we check wether a number is primary or not ? 
1. The algorith must check whether the number is a positive greater than one
2. The algorithm must check to see whether there are truly no other numbers that can divide that number other than itself
3. Number two must be considered as a primary number
*/

bool isPrime (int x) {
    if (x == 1) {
        return false;
    }
    for(int i = 2 ; i < x ; i++) {
        if(x % i == 0 ) {
            return false;
        }
    }
    return true;
}

int main() {
    int x;
    cin >> x;
    if(isPrime(x) == true) {
        cout << "Prime Number" << endl;        
    }
    else {
        cout << "Not a prime number" << endl;
    }
    return 0; 

}

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
#include <bits/stdc++.h>
using namespace std;

/* 
Problem 2 : You are given two positive integers , N and M Please calculate N^M mod 10^9

Constraint : 1 <= N, M <= 10^9 Time Limit : 1 Second
*/

int math(int n, int m) {
    return n^m % 10&9;
}

int main() {
	int n, m;
	cin >> n >> m;
	
    cout << math (n,m) << endl;
}

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
In competitive coding you need to focus more on algorithms instead of the language or formulas. You need to know how to translate the logic in your computer's codes, and if you already know how to do that, then you should be okay !


