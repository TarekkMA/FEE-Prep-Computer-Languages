## Chapter 2 Answers
***
** Questions index: **     
[1](#1) . [2](#2) . [3](#3) . [4](#4) . [5](#5) . [6](#6) . [7](#7) . [8](#8) . [9](#9) . [10](#10) . [11](#11) . [12](#12) . [13](#13) . [14](#14) . [15](#15) . [16](#16) . [17](#17)
***
#### 1.
**Write four different C++ statemnts, each subtracting 1 from the integer variable n.**
```cpp
// 1.
n = n-1;
// 2.
n --;
// 3.
n -= 1;
// 4.
n += -1;

```
#### 2.
**Without using the pre-increment operator, write a block of C++ code that has the same effect as the statement.**    
``` n = 100 + m++; ```
```cpp
n = 100 + m;
m = m + 1;
```
#### 3.
**Without using the pre-increment operator, write a block of C++ code that has the same effect as the statement.**     
``` n = 100 + ++m; ```
```cpp
m = m + 1;
n = 100 + m;
```
#### 4.
**Write a single C++ statement that subtracts the sum of x and y from z and then increments y.**
```cpp
result = z - ( x + y++)
```
#### 5.
**Write a single C++ statement that decrements the variable n and then adds it to total.**
```cpp
result =  --n + total;
```
#### 6.
**Write a program that prints the first sentence of the Gettysburg Address (or your favorite quotation).**
```cpp
#include <iostream>
using namespace std;

int main()
{
	cout << "\"Talk is cheap. Show me the code\" -Linus Torvalds" << endl;
	return 0;
}

```
#### 7.
**Write and run a program that prints the first letter of your last name as a block letter in a 7 × 7 grid of stars**    
السؤال دا هيعتمد علي إسمك بس أنا هيبقي حرف
A
```cpp
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
#### 8.
**Write a program that prints the block letter "B" in a 7 × 6 grid of stars like this : **
```cpp
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
#### 9.
**Write and run a program that shows what happens when each of the following ten "escape squences" is printed: ``\a`` ``\b`` ``\n`` ``\t`` ``\v`` ``\'`` ``\"`` ``\\`` ``\?``**
```cpp
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
#### 10.
**Write and run a program that prints the sum, diffrance, product, quitent, and the remainder of two integers. Initialize the integers with the values 60 and 7.**
```cpp
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
#### 11.
 **Write and run a program that prints the sum, diffrance, product, quitent, and the remainder of two integers that are input interactively.**
```cpp
#include <iostream>
using namespace std;

int main() {
	int num1;
	int num2;

	cout << "Enter the first number :";
	cin >> num1;
	cout << "Enter the second number :";
	cin >> num2;

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
#### 12.
** Write and run a test program that shows how your system handels uninitialized variables.**
```cpp
#include <iostream>
using namespace std;

int main() {
	bool b;
	char c;
	int i;
	float f;
	double d;
	cout << "Boolean :" << b << endl;
	cout << "Character :" << c << endl;
	cout << "Integer :" << i << endl;
	cout << "Float :" << f << endl;
	cout << "Double :" << d << endl;
}
```
#### 13.
**Write and run a program that causes negative overflow of a variable of type short.**
```cpp
#include <iostream>
using namespace std;

int main() {
	short num = 32767;
	cout << num << endl;
	num++;
	cout << num << endl;
	return 0;
}
```
#### 14.
**Write and rum a program like the one in Example 2.2 that prints the ASCII codes for only the 10 upper case and lower case vowels.**    
مش فاهم السؤال أوي  :sweat_smile:
شارك بالحل بتاعك علشان نضيفة هنا.

#### 15.
**Write a program that converts inches to centimeters For examplem if the user enters 16.9 for a length in inches the output would be 42.926 cm. (1 inch =2.54 centimeters)**
```cpp
#include <iostream>
using namespace std;

int main() {
	float in,cm;
	cout << "Enter lenght in inches :"
	cin >> in;
	cm = in * 2.54;
	cout << cm << " cm" << endl;
 	return 0;
}
```
#### 16.
**Write and run a program that reads the value of two floatsand outputs their sum, diffrance, product, quitent, and the remainder. Include a sensible input promt and informative output**    
```cpp
#include <iostream>
using namespace std;

int main() {
	cout << "Simple Calculator" << endl;

    float num1;
    int num2;

    cout << "Enter the first number :";
    cin >> num1;
    cout << "Enter the second number :";
    cin >> num2;

    float sum = num1 + num2;
    float diff = num1 - num2;
    float mul = num1 * num2;
    float div = num1 / num2;
    float ram = num1 % num2;

    cout << "Sum :" << sum << endl;
    cout << "Difference :" << diff << endl;
    cout << "Product :" << mul << endl;
    cout << "Quotient :" << div << endl;
    cout << "Remainder :" << ram << endl;
}
```
#### 17.
**Write a program to evaluate the fule consumption of a car. The mileage at the start and the end of the journey should be read, and also the fule level in the tank at the start and end of journey. Calculate fuel used, miles travelled, and hence the overall fule consumption in miles travelled per gallon of fuel.**    

```cpp
#include <iostream>
using namespace std;

int main() {

	float mileageS, mileageE;
	float fuleS, fuleE;
	float fuleUsed, milesTravelld, milePerFule;

	cout << "Enter mileage at the start :";
	cin >> mileageS;
	cout << "Enter Ending at the end :";
	cin >> mileageE;

	cout << "Enter fule at the start (liters):";
	cin >> fuleS;
	cout << "Enter fule at the end (liters):";
	cin >> fuleE;

	fuleUsed = fuleS - fuleE;
	milesTravelld = mileageE - mileageS;
	milePerFule = milesTravelld / fuleUsed;

	cout << "Fule used :" << fuleUsed << " liters." << endl;
	cout << "Miles travelled :" << milesTravelld << " miles." << endl;
	cout << "Miles travelled per fule liters :" << milePerFule << " miles/liter." << endl;


	return 0;
}
```
