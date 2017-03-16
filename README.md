# FEE Prep Computer Languages
**2016-2017 Book**
***
### **Contents :-**
*  :beginner: **Answers**
    * Chapter 1  :warning:
    * Chapter 2 
    * Chapter 3  :warning:
    * Chapter 4  :warning:
    * Chapter 5  :warning:
    * Chapter 6  :warning:

***
## Answers
### Chapter 1
_Under Construction_ :zzz:
### Chapter 2
1. Write four different C++ statemnts, each subtracting 1 from the integer variable n.
```c++
// 1.
n = n-1;
// 2.
n --;
// 3.
n -= 1;
// 4.
n += -1;

```
2. Without using the pre-increment operator, write a block of C++ code that has the same effect as the statement.    
``` n = 100 + m++; ```
```c++
n = 100 + m;
m = m + 1;
```
3. Without using the pre-increment operator, write a block of C++ code that has the same effect as the statement.     
``` n = 100 + ++m; ```
```c++
m = m + 1;
n = 100 + m;
```
4. Write a single C++ statement that subtracts the sum of x and y from z and then increments y.
```c++
result = z - ( x + y++)
```
5. Write a single C++ statement that decrements the variable n and then adds it to total.
```c++
result =  --n + total;
```
6. Write a program that prints the first sentence of the Gettysburg Address (or your favorite quotation).
```c++
#include <iostream>
using namespace std;

int main()
{
	cout << "\"Talk is cheap. Show me the code\" -Linus Torvalds" << endl;
	return 0;
}

```
7. Write and run a program that prints the first letter of your last name as a block letter in a 7 × 7 grid of stars
السؤال دا هيعتمد علي إسمك بس أنا هيبقي حرف A