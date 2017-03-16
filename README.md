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
#### **1)** Write four different C++ statemnts, each subtracting 1 from the integer variable n.
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
#### **2)** Without using the pre-increment operator, write a block of C++ code that has the same effect as the statement.    
``` n = 100 + m++; ```
```c++
n = 100 + m;
m = m + 1;
```
#### **3)** Without using the pre-increment operator, write a block of C++ code that has the same effect as the statement.     
``` n = 100 + ++m; ```
```c++
m = m + 1;
n = 100 + m;
```
#### **4)** Write a single C++ statement that subtracts the sum of x and y from z and then increments y.
```c++
result = z - ( x + y++)
```
#### **5)** Write a single C++ statement that decrements the variable n and then adds it to total.
```c++
result =  --n + total;
```
#### **6)** Write a program that prints the first sentence of the Gettysburg Address (or your favorite quotation).
```c++
#include <iostream>
using namespace std;

int main()
{
	cout << "\"Talk is cheap. Show me the code\" -Linus Torvalds" << endl;
	return 0;
}

```
#### **7)** Write and run a program that prints the first letter of your last name as a block letter in a 7 × 7 grid of stars
السؤال دا هيعتمد علي إسمك بس أنا هيبقي حرف 
A
```
#include <iostream>
using namespace std;

int main()
{
	cout << "*******" << endl;
	cout << "*     *" << endl;
	cout << "*     *" << endl;
	cout << "*******" << endl;
	cout << "*     *" << endl;
	cout << "*     *" << endl;
	cout << "*     *" << endl;
	return 0;
}

```
#### **8)** Write a program that prints the block letter "B" in a 7 × 6 grid of stars like this : 
```c++
#include <iostream>
using namespace std;

int main()
{
	cout << "*****" << endl;
	cout << "*    *" << endl;
	cout << "*    *" << endl;
	cout << "*****" << endl;
	cout << "*    *" << endl;
	cout << "*    *" << endl;
	cout << "*****" << endl;
	return 0;
}

```
#### **9)** Write and run a program that shows what happens when each of the following ten "escape squences" is printed: ``\a`` ``\b`` ``\n`` ``\t`` ``\v`` ``\'`` ``\"`` ``\\`` ``\?``
```c++
#include <iostream>
using namespace std;

int main() {
	cout << "Alert [Start]" << "\a" << "[End]" << endl; // This should play beeb sound
    cout << "Backspace [Start]" << "\b" << "[End]" << endl;
    cout << "New Line [Start]" << "\n" << "[End]" << endl;
	cout << "Carriage Return [Start]" << "\r" << "[End]" << endl;
    cout << "Horizontal Tab [Start]" << "\t" << "[End]" << endl;
	cout << "Vertical Tab [Start]" << "\v" << "[End]" << endl;
	cout << "Single Quote [Start]" << "\'" << "[End]" << endl;
	cout << "Double Quote [Start]" << "\"" << "[End]" << endl;
    cout << "Backslash [Start]" << "\\" << "[End]" << endl;
	cout << "Question Mark [Start]" << "\?" << "[End]" << endl;
}
```
#### **10)** Write and run a program that prints the sum, diffrance, product, quitent, and the remainder of two integers. Initialize the integers with the values 60 and 7.
```c++
#include <iostream>
using namespace std;

int main() {
	int num1 = 60;
	int num2 = 7;
	
	int sum = num1 + num2;
	int diff = num1 - num2;
	int mul = num1 * num2;
	int div = num1 / num2;
	int ram = num1 % num2;
	
	cout << "Sum :" << sum << endl;
	cout << "Difference :" << diff << endl;
	cout << "Product :" << mul << endl;
	cout << "Quotient :" << div << endl;
	cout << "Remainder :" << ram << endl;
}
```
#### **11)**  