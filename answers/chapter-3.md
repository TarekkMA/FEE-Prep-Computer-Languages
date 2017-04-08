## Chapter 2 Answers
***
**Questions index:**
[1](#1) . [2](#2) . [3](#3) . [4](#4) . [5](#5) . [6](#6) . [7](#7) . [8](#8) . [9](#9) . [10](#10) . [11](#11)
***
#### 1.
**Modify the program in Example 3.1 so that it prints a response only if n is divisible by d.**    
````cpp
int main()
int main() {
	int n, d;
	cout << "Enter two positive integers: ";
	cin >> n >> d;
	if (n%d == 0) cout << n << " is not divisible by " << d << endl;
}
````
#### 2.
**Modify the program in Example 3.1 so that it prints the minimum of four input integers**
````cpp
int main() {
	int n1,n2,n3,n4;
	cout << "Enter 4 integers: ";
	cin >> n1 >> n2 >> n3 >> n4;
	int min = n1;
	if (n2 < min) min = n2;
	if (n3 < min) min = n3;
	if (n4 < min) min = n4;
	cout << "Their minimum is " << min << endl;
}
````
#### 3.
````cpp

````
