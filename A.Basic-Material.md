# 🚀 Competitive Programming Notes (C++)

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

## C.Operator
Operators are just basically math equation that you usually see everywhere.
